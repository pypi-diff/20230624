# Comparing `tmp/pytrimal-0.5.5.tar.gz` & `tmp/pytrimal-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrimal-0.5.5.tar", last modified: Mon Oct 17 13:06:57 2022, max compression
+gzip compressed data, was "pytrimal-0.6.0.tar", last modified: Sat Jun 24 10:15:16 2023, max compression
```

## Comparing `pytrimal-0.5.5.tar` & `pytrimal-0.6.0.tar`

### file list

```diff
@@ -1,387 +1,344 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:57.111421 pytrimal-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (121)     6118 2022-10-17 13:06:38.000000 pytrimal-0.5.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-10-17 13:06:38.000000 pytrimal-0.5.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    35148 2022-10-17 13:06:38.000000 pytrimal-0.5.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-10-17 13:06:38.000000 pytrimal-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12911 2022-10-17 13:06:57.111421 pytrimal-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11171 2022-10-17 13:06:38.000000 pytrimal-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.963420 pytrimal-0.5.5/include/
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-10-17 13:06:38.000000 pytrimal-0.5.5/include/_unicode.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.963420 pytrimal-0.5.5/include/cpu_features/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:38.000000 pytrimal-0.5.5/include/cpu_features/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-10-17 13:06:38.000000 pytrimal-0.5.5/include/cpu_features/aarch64.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-10-17 13:06:38.000000 pytrimal-0.5.5/include/cpu_features/arm.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-10-17 13:06:38.000000 pytrimal-0.5.5/include/cpu_features/x86.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-10-17 13:06:38.000000 pytrimal-0.5.5/include/iostream.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.963420 pytrimal-0.5.5/include/trimal/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-17 13:06:38.000000 pytrimal-0.5.5/include/trimal/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2334 2022-10-17 13:06:38.000000 pytrimal-0.5.5/include/trimal/alignment.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-10-17 13:06:38.000000 pytrimal-0.5.5/include/trimal/cleaner.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-10-17 13:06:38.000000 pytrimal-0.5.5/include/trimal/format_handling.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2192 2022-10-17 13:06:38.000000 pytrimal-0.5.5/include/trimal/manager.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     8874 2022-10-17 13:06:38.000000 pytrimal-0.5.5/include/trimal/report_system.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-10-17 13:06:38.000000 pytrimal-0.5.5/include/trimal/sequences_matrix.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-10-17 13:06:38.000000 pytrimal-0.5.5/include/trimal/similarity_matrix.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-10-17 13:06:38.000000 pytrimal-0.5.5/include/trimal/statistics.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.967420 pytrimal-0.5.5/patches/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/BaseFormatHandler.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/Cleaner.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/Cleaner.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/Gaps.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/Similarity.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/clustal_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/clustal_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/fasta_m10_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/fasta_m10_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/fasta_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/fasta_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/htmlreport_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/htmlreport_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/mega_interleaved_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/mega_interleaved_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/mega_sequential_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/mega_sequential_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/nexus_m10_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/nexus_m10_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/nexus_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/nexus_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/phylip32_m10_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/phylip32_m10_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/phylip32_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/phylip32_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/phylip40_m10_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/phylip40_m10_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/phylip40_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/phylip40_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/phylip_paml_m10_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/phylip_paml_m10_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/phylip_paml_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/phylip_paml_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)      944 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/pir_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/pir_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/similarityMatrix.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-10-17 13:06:38.000000 pytrimal-0.5.5/patches/trimalManager.h.patch
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-10-17 13:06:56.000000 pytrimal-0.5.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.971420 pytrimal-0.5.5/pytrimal/
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3822 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/_trimal.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     6424 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/_trimal.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    79341 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/_trimal.pyx
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.971420 pytrimal-0.5.5/pytrimal/fileobj/
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/fileobj/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/fileobj/pyreadbuf.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/fileobj/pyreadbuf.h
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/fileobj/pyreadintobuf.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/fileobj/pyreadintobuf.h
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/fileobj/pywritebuf.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/fileobj/pywritebuf.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.975420 pytrimal-0.5.5/pytrimal/impl/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3221 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/avx.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/avx.h
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/avx.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2883 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/generic.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/generic.h
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/generic.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3164 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/mmx.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/mmx.h
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/mmx.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3182 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/neon.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/neon.h
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/neon.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3095 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/sse.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/sse.h
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/sse.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    20440 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/impl/template.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.975420 pytrimal-0.5.5/pytrimal/patch/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/patch/omp.h
--rw-r--r--   0 runner    (1001) docker     (121)     6449 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/patch/reportsystem.cpp
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.975420 pytrimal-0.5.5/pytrimal/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.983420 pytrimal-0.5.5/pytrimal/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)   178679 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.automated1.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    10138 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.clusters10.fasta
--rw-r--r--   0 runner    (1001) docker     (121)     4892 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.clusters5.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   180351 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.cons40.gt40.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   161541 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.cons60.gt90.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   266668 2022-10-17 13:06:41.000000 pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   178679 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.gappyout.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    13677 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.id50.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    73561 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.id70.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    97956 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.maxidentity75.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   265832 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.noallgaps.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   264560 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.noduplicateseqs.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   265832 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.seq40.res60.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   214721 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.seq80.res80.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   148792 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.strict.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   129773 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.strictplus.fasta
--rw-r--r--   0 runner    (1001) docker     (121)     2766 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/PF12574.full.afa
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-10-17 13:06:40.000000 pytrimal-0.5.5/pytrimal/tests/data/example.001.AA.clw
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/example.001.gt90.w3.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   142966 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/halorhodopsin.afa
--rw-r--r--   0 runner    (1001) docker     (121)     3187 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/data/pam70.json
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)    14042 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/test_alignment.py
--rw-r--r--   0 runner    (1001) docker     (121)     5480 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/test_automatic_trimmer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/test_doctest.py
--rw-r--r--   0 runner    (1001) docker     (121)     5408 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/test_manual_trimmer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3510 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/test_overlap_trimmer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4355 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/test_representative_trimmer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-10-17 13:06:38.000000 pytrimal-0.5.5/pytrimal/tests/test_similarity_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.971420 pytrimal-0.5.5/pytrimal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12911 2022-10-17 13:06:56.000000 pytrimal-0.5.5/pytrimal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15603 2022-10-17 13:06:56.000000 pytrimal-0.5.5/pytrimal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 13:06:56.000000 pytrimal-0.5.5/pytrimal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 13:06:56.000000 pytrimal-0.5.5/pytrimal.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-17 13:06:56.000000 pytrimal-0.5.5/pytrimal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3001 2022-10-17 13:06:57.111421 pytrimal-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    30309 2022-10-17 13:06:38.000000 pytrimal-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.959420 pytrimal-0.5.5/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.983420 pytrimal-0.5.5/vendor/cpu_features/
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    12876 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8068 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.983420 pytrimal-0.5.5/vendor/cpu_features/ci/
--rw-r--r--   0 runner    (1001) docker     (121)     2896 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/ci/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.983420 pytrimal-0.5.5/vendor/cpu_features/cmake/
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/cmake/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.983420 pytrimal-0.5.5/vendor/cpu_features/include/
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/include/cpu_features_cache_info.h
--rw-r--r--   0 runner    (1001) docker     (121)     7081 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/include/cpu_features_macros.h
--rw-r--r--   0 runner    (1001) docker     (121)     5451 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/include/cpuinfo_aarch64.h
--rw-r--r--   0 runner    (1001) docker     (121)     3723 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/include/cpuinfo_arm.h
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/include/cpuinfo_mips.h
--rw-r--r--   0 runner    (1001) docker     (121)     4493 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/include/cpuinfo_ppc.h
--rw-r--r--   0 runner    (1001) docker     (121)     6650 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/include/cpuinfo_x86.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.987420 pytrimal-0.5.5/vendor/cpu_features/include/internal/
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/include/internal/bit_utils.h
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/include/internal/cpuid_x86.h
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/include/internal/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (121)     7085 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/include/internal/hwcaps.h
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/include/internal/stack_line_reader.h
--rw-r--r--   0 runner    (1001) docker     (121)     4127 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/include/internal/string_view.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.987420 pytrimal-0.5.5/vendor/cpu_features/ndk_compat/
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/ndk_compat/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.987420 pytrimal-0.5.5/vendor/cpu_features/src/
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/copy.inl
--rw-r--r--   0 runner    (1001) docker     (121)     3126 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/define_introspection.inl
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/define_introspection_and_hwcaps.inl
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/equals.inl
--rw-r--r--   0 runner    (1001) docker     (121)     1808 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/filesystem.c
--rw-r--r--   0 runner    (1001) docker     (121)     5177 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/hwcaps.c
--rw-r--r--   0 runner    (1001) docker     (121)     7686 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/impl_aarch64_linux_or_android.c
--rw-r--r--   0 runner    (1001) docker     (121)     9080 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/impl_arm_linux_or_android.c
--rw-r--r--   0 runner    (1001) docker     (121)     3142 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/impl_mips_linux_or_android.c
--rw-r--r--   0 runner    (1001) docker     (121)     7876 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/impl_ppc_linux.c
--rw-r--r--   0 runner    (1001) docker     (121)    76257 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/impl_x86__base_implementation.inl
--rw-r--r--   0 runner    (1001) docker     (121)     2660 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/impl_x86_freebsd.c
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/impl_x86_linux_or_android.c
--rw-r--r--   0 runner    (1001) docker     (121)     2173 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/impl_x86_macos.c
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/impl_x86_windows.c
--rw-r--r--   0 runner    (1001) docker     (121)     4136 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/stack_line_reader.c
--rw-r--r--   0 runner    (1001) docker     (121)     6603 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/string_view.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.987420 pytrimal-0.5.5/vendor/cpu_features/src/utils/
--rw-r--r--   0 runner    (1001) docker     (121)    13848 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/cpu_features/src/utils/list_cpu_features.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:56.991420 pytrimal-0.5.5/vendor/trimal/
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     6237 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:57.091421 pytrimal-0.5.5/vendor/trimal/dataset/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/alignments_comparison.1
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/alignments_comparison.2
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/alignments_comparison.3
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.001.AA.clw
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.001.AA.msl
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.001.AA.phy
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.002.AA.clw
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.002.AA.phy
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.003.AA.clw
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.004.AA.fasta
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.005.AA.fasta
--rw-r--r--   0 runner    (1001) docker     (121)     2451 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.006.AA.pir
--rw-r--r--   0 runner    (1001) docker     (121)    29920 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.007.AA.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    14306 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.007.AA.only_seqs
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.009.AA.fasta
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.010.AA.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    64904 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.011.AA.YKL197C.clw
--rw-r--r--   0 runner    (1001) docker     (121)    41006 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.011.AA.YKL197C.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    40853 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.011.AA.YKL197C.phy
--rw-r--r--   0 runner    (1001) docker     (121)  2265147 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.012.AA.SuperAlignment.phy
--rw-r--r--   0 runner    (1001) docker     (121)  1246007 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.013.AA.SuperAlignment.phy
--rw-r--r--   0 runner    (1001) docker     (121) 26589443 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.014.AA.EggNOG.COG0591.fasta
--rw-r--r--   0 runner    (1001) docker     (121) 12097211 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.015.AA.bctoNOG.ENOG41099F3.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   276588 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.016.AA.bctoNOG.ENOG41099FB.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   138345 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.017.AA.bctoNOG.ENOG41099FJ.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   203668 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.018.AA.bctoNOG.ENOG41099FV.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   377416 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.019.AA.bctoNOG.ENOG41099HI.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   453386 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.020.AA.bctoNOG.ENOG41099HN.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   116996 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.021.AA.bctoNOG.ENOG41099I5.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   155773 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.022.AA.bctoNOG.ENOG41099IZ.fasta
--rw-r--r--   0 runner    (1001) docker     (121)  2785573 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.023.AA.bctoNOG.ENOG41099K3.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    13444 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.024.AA.bctoNOG.ENOG41099KM.fasta
--rw-r--r--   0 runner    (1001) docker     (121)  1608238 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.025.AA.bctoNOG.ENOG41099KP.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   568299 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.026.AA.bctoNOG.ENOG41099MV.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    50764 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.027.AA.bctoNOG.ENOG41099NY.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   591641 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.028.AA.bctoNOG.ENOG41099PA.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   139720 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.029.AA.bctoNOG.ENOG41099Q3.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   186348 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.030.AA.bctoNOG.ENOG41099RG.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   212250 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.031.AA.bctoNOG.ENOG41099UK.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   387866 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.032.AA.bctoNOG.ENOG41099UW.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   492698 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.033.AA.bctoNOG.ENOG41099VK.fasta
--rw-r--r--   0 runner    (1001) docker     (121)  1613156 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.034.AA.bctoNOG.ENOG41099WA.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   610988 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.035.AA.bctoNOG.ENOG41099WF.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   119286 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.036.AA.bctoNOG.ENOG41099XJ.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   230484 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.037.AA.bctoNOG.ENOG41099XP.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   261077 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.038.AA.bctoNOG.ENOG41099Y4.fasta
--rw-r--r--   0 runner    (1001) docker     (121)  3740628 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.039.AA.bctoNOG.ENOG41099YD.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   506035 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.040.AA.bctoNOG.ENOG4109A32.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    58122 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.041.AA.bctoNOG.ENOG4109A5T.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    92703 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.042.AA.bctoNOG.ENOG4109A9M.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    32257 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.043.AA.bctoNOG.ENOG4109ADN.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    77067 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.044.AA.bctoNOG.ENOG4109AED.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    22315 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.045.AA.bctoNOG.ENOG4109AGT.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    22046 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.046.AA.bctoNOG.ENOG4109AGW.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    22523 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.047.AA.bctoNOG.ENOG4109AIC.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    15267 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.048.AA.bctoNOG.ENOG4109AJ3.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    22263 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.049.AA.bctoNOG.ENOG4109AY5.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    16768 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.050.AA.bctoNOG.ENOG4109B8Z.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    35547 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.051.AA.bctoNOG.ENOG4109BCJ.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    34229 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.052.AA.bctoNOG.ENOG4109CTU.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    11810 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.053.AA.bctoNOG.ENOG4109CVC.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    26156 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.054.AA.bctoNOG.ENOG4109FIT.fasta
--rw-r--r--   0 runner    (1001) docker     (121)     5970 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.055.AA.bctoNOG.ENOG4109GY9.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    14878 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.056.AA.bctoNOG.ENOG4109IPJ.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    55278 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.057.AA.bctoNOG.ENOG4109SZ2.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    15249 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.058.AA.strNOG.ENOG411BBR6.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    16927 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.059.AA.strNOG.ENOG411BBRR.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    59625 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.060.AA.strNOG.ENOG411BBWK.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    50162 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.061.AA.strNOG.ENOG411BCDZ.fasta
--rw-r--r--   0 runner    (1001) docker     (121)  1153350 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.062.AA.strNOG.ENOG411BCX3.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    20437 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.063.AA.strNOG.ENOG411BDBU.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   247440 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.064.AA.strNOG.ENOG411BDKC.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    47806 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.065.AA.strNOG.ENOG411BDSZ.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    27309 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.066.AA.strNOG.ENOG411BDUE.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    51327 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.067.AA.strNOG.ENOG411BDX3.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    16203 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.068.AA.strNOG.ENOG411BE45.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    21963 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.069.AA.strNOG.ENOG411BE8B.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    61363 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.070.AA.strNOG.ENOG411BEUV.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    55532 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.071.AA.strNOG.ENOG411BEZ0.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    11957 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.072.AA.strNOG.ENOG411BF1S.fasta
--rw-r--r--   0 runner    (1001) docker     (121)  2483264 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.073.AA.strNOG.ENOG411BFCW.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    25440 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.074.AA.strNOG.ENOG411BFPF.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    19199 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.075.AA.strNOG.ENOG411BFQS.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    33482 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.076.AA.strNOG.ENOG411BH75.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    72534 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.077.AA.strNOG.ENOG411BH79.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    44284 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.078.AA.strNOG.ENOG411BH99.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    13755 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.079.AA.strNOG.ENOG411BJDC.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    23290 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.080.AA.strNOG.ENOG411BJIF.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    12036 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.081.AA.strNOG.ENOG411BK9X.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    26165 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.082.AA.strNOG.ENOG411BKC5.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    13968 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.083.AA.strNOG.ENOG411BMKC.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    10016 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.084.AA.strNOG.ENOG411BNP9.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    10739 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.085.AA.strNOG.ENOG411BQTJ.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    25977 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.086.AA.strNOG.ENOG411BR1D.fasta
--rw-r--r--   0 runner    (1001) docker     (121)     7768 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.087.AA.strNOG.ENOG411BRCH.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    15763 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.088.AA.strNOG.ENOG411BSXF.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    11736 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.089.AA.strNOG.ENOG411BV9B.fasta
--rw-r--r--   0 runner    (1001) docker     (121)  1574791 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.090.AA.strNOG.ENOG411BVKR.fasta
--rw-r--r--   0 runner    (1001) docker     (121)   473273 2022-10-17 13:06:40.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.091.AA.strNOG.ENOG411BWBU.codon.fa
--rw-r--r--   0 runner    (1001) docker     (121)   266668 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.091.AA.strNOG.ENOG411BWBU.fasta
--rw-r--r--   0 runner    (1001) docker     (121)     4890 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.092.DNA.fasta
--rw-r--r--   0 runner    (1001) docker     (121)     4848 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.093.DNA.fasta
--rw-r--r--   0 runner    (1001) docker     (121)    10293 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/dataset/example.094.DNADeg.sequential_phy
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/dataset/matrix.BLOSUM62
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/dataset/matrix.Degenerated_DNA
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:57.095421 pytrimal-0.5.5/vendor/trimal/include/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:57.095421 pytrimal-0.5.5/vendor/trimal/include/Alignment/
--rw-r--r--   0 runner    (1001) docker     (121)     3823 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/Alignment/Alignment.h
--rw-r--r--   0 runner    (1001) docker     (121)     5402 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/Alignment/sequencesMatrix.h
--rw-r--r--   0 runner    (1001) docker     (121)    20122 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/Cleaner.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:57.095421 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/
--rw-r--r--   0 runner    (1001) docker     (121)     4572 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/BaseFormatHandler.h
--rw-r--r--   0 runner    (1001) docker     (121)     8554 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/FormatManager.h
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/clustal_state.h
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/fasta_m10_state.h
--rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/fasta_state.h
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/formats_header.h
--rw-r--r--   0 runner    (1001) docker     (121)     1883 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/htmlreport_state.h
--rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/mega_interleaved_state.h
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/mega_sequential_state.h
--rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/nexus_m10_state.h
--rw-r--r--   0 runner    (1001) docker     (121)     1875 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/nexus_state.h
--rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/phylip32_m10_state.h
--rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/phylip32_state.h
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/phylip40_m10_state.h
--rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/phylip40_state.h
--rw-r--r--   0 runner    (1001) docker     (121)     1926 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/phylip_paml_m10_state.h
--rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/phylip_paml_state.h
--rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/FormatHandling/pir_state.h
--rw-r--r--   0 runner    (1001) docker     (121)     4773 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/InternalBenchmarker.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:57.095421 pytrimal-0.5.5/vendor/trimal/include/RawText/
--rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/RawText/examples.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11662 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/RawText/legacyMenu.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13285 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/RawText/menu.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:57.099421 pytrimal-0.5.5/vendor/trimal/include/Statistics/
--rw-r--r--   0 runner    (1001) docker     (121)     7931 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/Statistics/Consistency.h
--rw-r--r--   0 runner    (1001) docker     (121)     2823 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/Statistics/Gaps.h
--rw-r--r--   0 runner    (1001) docker     (121)     4871 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/Statistics/Manager.h
--rw-r--r--   0 runner    (1001) docker     (121)     2653 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/Statistics/Mold.h
--rw-r--r--   0 runner    (1001) docker     (121)     4935 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/Statistics/Similarity.h
--rw-r--r--   0 runner    (1001) docker     (121)     4262 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/Statistics/similarityMatrix.h
--rw-r--r--   0 runner    (1001) docker     (121)     9689 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/VCFHandler.h
--rw-r--r--   0 runner    (1001) docker     (121)     3357 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/defines.h
--rw-r--r--   0 runner    (1001) docker     (121)    18611 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/reportsystem.h
--rw-r--r--   0 runner    (1001) docker     (121)    13715 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/trimalManager.h
--rw-r--r--   0 runner    (1001) docker     (121)    15362 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/utils.h
--rw-r--r--   0 runner    (1001) docker     (121)     6542 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/include/values.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:57.099421 pytrimal-0.5.5/vendor/trimal/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:57.103421 pytrimal-0.5.5/vendor/trimal/source/Alignment/
--rw-r--r--   0 runner    (1001) docker     (121)   100282 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/Alignment/Alignment.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8035 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/Alignment/sequencesMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    66998 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/Cleaner.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:57.107421 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/
--rw-r--r--   0 runner    (1001) docker     (121)    12834 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/BaseFormatHandler.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    10418 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/clustal_state.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4774 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/fasta_m10_state.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     7827 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/fasta_state.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     5265 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/htmlreport_state.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8309 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/mega_interleaved_state.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    11393 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/mega_sequential_state.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6813 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/nexus_m10_state.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    11783 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/nexus_state.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4753 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/phylip32_m10_state.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    11330 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/phylip32_state.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/phylip40_m10_state.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    10907 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/phylip40_state.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3927 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/phylip_paml_m10_state.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3604 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/phylip_paml_state.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8406 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/pir_state.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    16449 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/FormatHandling/readAlMain.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6977 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/InternalBenchmarker.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:57.107421 pytrimal-0.5.5/vendor/trimal/source/Statistics/
--rw-r--r--   0 runner    (1001) docker     (121)    32843 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/Statistics/Consistency.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    24994 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/Statistics/Gaps.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     7798 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/Statistics/Manager.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    13643 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/Statistics/Mold.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    24884 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/Statistics/Similarity.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    16144 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/Statistics/similarityMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    25928 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/VCFHandler.cpp
--rw-r--r--   0 runner    (1001) docker     (121)   126562 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/alignment.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    21325 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/compareFiles.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    90551 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:06:57.111421 pytrimal-0.5.5/vendor/trimal/source/reportMessages/
--rw-r--r--   0 runner    (1001) docker     (121)    17145 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/reportMessages/errorMessages.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/reportMessages/infoMessages.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2755 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/reportMessages/warningMessages.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8144 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/reportsystem.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    71034 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/rwAlignment.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2485 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/trimAlMain.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    84059 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/trimalManager.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2342 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/typeHelper.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    30036 2022-10-17 13:06:41.000000 pytrimal-0.5.5/vendor/trimal/source/utils.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.979654 pytrimal-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-24 10:15:04.000000 pytrimal-0.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-24 10:15:04.000000 pytrimal-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-24 10:15:04.000000 pytrimal-0.6.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-24 10:15:04.000000 pytrimal-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-06-24 10:15:16.979654 pytrimal-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-06-24 10:15:04.000000 pytrimal-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.887648 pytrimal-0.6.0/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/_unicode.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.887648 pytrimal-0.6.0/include/cpu_features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/cpu_features/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/cpu_features/aarch64.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/cpu_features/arm.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/cpu_features/x86.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/iostream.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.887648 pytrimal-0.6.0/include/trimal/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/alignment.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/cleaner.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/format_handling.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/report_system.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/sequences_matrix.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/similarity_matrix.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/statistics.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.891649 pytrimal-0.6.0/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/BaseFormatHandler.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/Cleaner.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/Cleaner.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/Gaps.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/Similarity.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/clustal_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/clustal_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/fasta_m10_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/fasta_m10_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/fasta_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/fasta_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/htmlreport_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/htmlreport_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/mega_interleaved_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/mega_interleaved_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/mega_sequential_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/mega_sequential_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/nexus_m10_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/nexus_m10_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/nexus_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/nexus_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip32_m10_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip32_m10_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip32_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip32_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip40_m10_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip40_m10_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip40_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip40_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip_paml_m10_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip_paml_m10_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip_paml_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip_paml_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/pir_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/pir_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/similarityMatrix.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/trimalManager.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-24 10:15:16.000000 pytrimal-0.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.891649 pytrimal-0.6.0/pytrimal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/_trimal.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/_trimal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    79527 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/_trimal.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.891649 pytrimal-0.6.0/pytrimal/fileobj/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/fileobj/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/fileobj/pyreadbuf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/fileobj/pyreadbuf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/fileobj/pyreadintobuf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/fileobj/pyreadintobuf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/fileobj/pywritebuf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/fileobj/pywritebuf.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.891649 pytrimal-0.6.0/pytrimal/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/avx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/avx.h
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/avx.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/generic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/generic.h
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/generic.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/mmx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/mmx.h
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/mmx.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/neon.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/neon.h
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/neon.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/sse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/sse.h
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/sse.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    20527 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/template.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.891649 pytrimal-0.6.0/pytrimal/patch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/patch/omp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/patch/reportsystem.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.895649 pytrimal-0.6.0/pytrimal/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.899649 pytrimal-0.6.0/pytrimal/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   178679 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.automated1.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.clusters10.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.clusters5.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   180351 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.cons40.gt40.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   161541 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.cons60.gt90.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   266668 2023-06-24 10:15:06.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   178679 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.gappyout.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.id50.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    73561 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.id70.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    97956 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.maxidentity75.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   265832 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.noallgaps.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   264560 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.noduplicateseqs.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   265832 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.seq40.res60.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   214721 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.seq80.res80.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   148792 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.strict.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   129773 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.strictplus.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/PF12574.full.afa
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-24 10:15:06.000000 pytrimal-0.6.0/pytrimal/tests/data/example.001.AA.clw
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/example.001.gt90.w3.clw
+-rw-r--r--   0 runner    (1001) docker     (123)   142966 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/halorhodopsin.afa
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/pam70.json
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14042 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/test_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/test_automatic_trimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/test_manual_trimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/test_overlap_trimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/test_representative_trimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/test_similarity_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.891649 pytrimal-0.6.0/pytrimal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-06-24 10:15:16.000000 pytrimal-0.6.0/pytrimal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-06-24 10:15:16.000000 pytrimal-0.6.0/pytrimal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 10:15:16.000000 pytrimal-0.6.0/pytrimal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 10:15:16.000000 pytrimal-0.6.0/pytrimal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-24 10:15:16.000000 pytrimal-0.6.0/pytrimal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 10:15:16.000000 pytrimal-0.6.0/pytrimal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-24 10:15:16.979654 pytrimal-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    29800 2023-06-24 10:15:04.000000 pytrimal-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.883648 pytrimal-0.6.0/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.899649 pytrimal-0.6.0/vendor/trimal/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.971654 pytrimal-0.6.0/vendor/trimal/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/alignments_comparison.1
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/alignments_comparison.2
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/alignments_comparison.3
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.001.AA.clw
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.001.AA.msl
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.001.AA.phy
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.002.AA.clw
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.002.AA.phy
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.003.AA.clw
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.004.AA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.005.AA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.006.AA.pir
+-rw-r--r--   0 runner    (1001) docker     (123)    29920 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.007.AA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.007.AA.only_seqs
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.009.AA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.010.AA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    64904 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.011.AA.YKL197C.clw
+-rw-r--r--   0 runner    (1001) docker     (123)    41006 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.011.AA.YKL197C.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    40853 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.011.AA.YKL197C.phy
+-rw-r--r--   0 runner    (1001) docker     (123)  2265147 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.012.AA.SuperAlignment.phy
+-rw-r--r--   0 runner    (1001) docker     (123)  1246007 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.013.AA.SuperAlignment.phy
+-rw-r--r--   0 runner    (1001) docker     (123) 26589443 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.014.AA.EggNOG.COG0591.fasta
+-rw-r--r--   0 runner    (1001) docker     (123) 12097211 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.015.AA.bctoNOG.ENOG41099F3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   276588 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.016.AA.bctoNOG.ENOG41099FB.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   138345 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.017.AA.bctoNOG.ENOG41099FJ.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   203668 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.018.AA.bctoNOG.ENOG41099FV.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   377416 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.019.AA.bctoNOG.ENOG41099HI.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   453386 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.020.AA.bctoNOG.ENOG41099HN.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   116996 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.021.AA.bctoNOG.ENOG41099I5.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   155773 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.022.AA.bctoNOG.ENOG41099IZ.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)  2785573 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.023.AA.bctoNOG.ENOG41099K3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    13444 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.024.AA.bctoNOG.ENOG41099KM.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)  1608238 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.025.AA.bctoNOG.ENOG41099KP.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   568299 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.026.AA.bctoNOG.ENOG41099MV.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    50764 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.027.AA.bctoNOG.ENOG41099NY.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   591641 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.028.AA.bctoNOG.ENOG41099PA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   139720 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.029.AA.bctoNOG.ENOG41099Q3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   186348 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.030.AA.bctoNOG.ENOG41099RG.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   212250 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.031.AA.bctoNOG.ENOG41099UK.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   387866 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.032.AA.bctoNOG.ENOG41099UW.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   492698 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.033.AA.bctoNOG.ENOG41099VK.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)  1613156 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.034.AA.bctoNOG.ENOG41099WA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   610988 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.035.AA.bctoNOG.ENOG41099WF.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   119286 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.036.AA.bctoNOG.ENOG41099XJ.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   230484 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.037.AA.bctoNOG.ENOG41099XP.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   261077 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.038.AA.bctoNOG.ENOG41099Y4.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)  3740628 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.039.AA.bctoNOG.ENOG41099YD.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   506035 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.040.AA.bctoNOG.ENOG4109A32.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    58122 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.041.AA.bctoNOG.ENOG4109A5T.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    92703 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.042.AA.bctoNOG.ENOG4109A9M.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    32257 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.043.AA.bctoNOG.ENOG4109ADN.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    77067 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.044.AA.bctoNOG.ENOG4109AED.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    22315 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.045.AA.bctoNOG.ENOG4109AGT.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    22046 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.046.AA.bctoNOG.ENOG4109AGW.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.047.AA.bctoNOG.ENOG4109AIC.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.048.AA.bctoNOG.ENOG4109AJ3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    22263 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.049.AA.bctoNOG.ENOG4109AY5.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.050.AA.bctoNOG.ENOG4109B8Z.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    35547 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.051.AA.bctoNOG.ENOG4109BCJ.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    34229 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.052.AA.bctoNOG.ENOG4109CTU.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.053.AA.bctoNOG.ENOG4109CVC.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    26156 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.054.AA.bctoNOG.ENOG4109FIT.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.055.AA.bctoNOG.ENOG4109GY9.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.056.AA.bctoNOG.ENOG4109IPJ.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    55278 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.057.AA.bctoNOG.ENOG4109SZ2.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.058.AA.strNOG.ENOG411BBR6.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    16927 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.059.AA.strNOG.ENOG411BBRR.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    59625 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.060.AA.strNOG.ENOG411BBWK.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    50162 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.061.AA.strNOG.ENOG411BCDZ.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)  1153350 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.062.AA.strNOG.ENOG411BCX3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.063.AA.strNOG.ENOG411BDBU.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   247440 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.064.AA.strNOG.ENOG411BDKC.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    47806 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.065.AA.strNOG.ENOG411BDSZ.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    27309 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.066.AA.strNOG.ENOG411BDUE.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    51327 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.067.AA.strNOG.ENOG411BDX3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.068.AA.strNOG.ENOG411BE45.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    21963 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.069.AA.strNOG.ENOG411BE8B.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    61363 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.070.AA.strNOG.ENOG411BEUV.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    55532 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.071.AA.strNOG.ENOG411BEZ0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.072.AA.strNOG.ENOG411BF1S.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)  2483264 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.073.AA.strNOG.ENOG411BFCW.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    25440 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.074.AA.strNOG.ENOG411BFPF.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.075.AA.strNOG.ENOG411BFQS.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    33482 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.076.AA.strNOG.ENOG411BH75.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    72534 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.077.AA.strNOG.ENOG411BH79.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    44284 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.078.AA.strNOG.ENOG411BH99.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.079.AA.strNOG.ENOG411BJDC.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.080.AA.strNOG.ENOG411BJIF.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.081.AA.strNOG.ENOG411BK9X.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    26165 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.082.AA.strNOG.ENOG411BKC5.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.083.AA.strNOG.ENOG411BMKC.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    10016 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.084.AA.strNOG.ENOG411BNP9.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.085.AA.strNOG.ENOG411BQTJ.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    25977 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.086.AA.strNOG.ENOG411BR1D.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.087.AA.strNOG.ENOG411BRCH.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.088.AA.strNOG.ENOG411BSXF.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.089.AA.strNOG.ENOG411BV9B.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)  1574791 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.090.AA.strNOG.ENOG411BVKR.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   473273 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.091.AA.strNOG.ENOG411BWBU.codon.fa
+-rw-r--r--   0 runner    (1001) docker     (123)   266668 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.091.AA.strNOG.ENOG411BWBU.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.092.DNA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.093.DNA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.094.DNADeg.sequential_phy
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/matrix.BLOSUM62
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/matrix.Degenerated_DNA
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.971654 pytrimal-0.6.0/vendor/trimal/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.971654 pytrimal-0.6.0/vendor/trimal/include/Alignment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Alignment/Alignment.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Alignment/sequencesMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20122 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Cleaner.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.971654 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/BaseFormatHandler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/FormatManager.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/clustal_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/fasta_m10_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/fasta_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/formats_header.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/htmlreport_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/mega_interleaved_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/mega_sequential_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/nexus_m10_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/nexus_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip32_m10_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip32_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip40_m10_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip40_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip_paml_m10_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip_paml_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/pir_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/InternalBenchmarker.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.971654 pytrimal-0.6.0/vendor/trimal/include/RawText/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/RawText/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/RawText/legacyMenu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/RawText/menu.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.975654 pytrimal-0.6.0/vendor/trimal/include/Statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Statistics/Consistency.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Statistics/Gaps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Statistics/Manager.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Statistics/Mold.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Statistics/Similarity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Statistics/similarityMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/VCFHandler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/defines.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/reportsystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/trimalManager.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15362 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/values.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.975654 pytrimal-0.6.0/vendor/trimal/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.975654 pytrimal-0.6.0/vendor/trimal/source/Alignment/
+-rw-r--r--   0 runner    (1001) docker     (123)   100282 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Alignment/Alignment.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Alignment/sequencesMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    66998 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Cleaner.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.975654 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/
+-rw-r--r--   0 runner    (1001) docker     (123)    12834 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/BaseFormatHandler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/clustal_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/fasta_m10_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/fasta_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/htmlreport_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/mega_interleaved_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/mega_sequential_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/nexus_m10_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/nexus_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip32_m10_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip32_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip40_m10_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip40_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip_paml_m10_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip_paml_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/pir_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16449 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/readAlMain.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/InternalBenchmarker.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.979654 pytrimal-0.6.0/vendor/trimal/source/Statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)    32843 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Statistics/Consistency.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Statistics/Gaps.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Statistics/Manager.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Statistics/Mold.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24884 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Statistics/Similarity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Statistics/similarityMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/VCFHandler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   126562 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/alignment.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21325 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/compareFiles.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    90551 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.979654 pytrimal-0.6.0/vendor/trimal/source/reportMessages/
+-rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/reportMessages/errorMessages.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/reportMessages/infoMessages.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/reportMessages/warningMessages.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/reportsystem.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    71034 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/rwAlignment.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/trimAlMain.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    84059 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/trimalManager.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/typeHelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/utils.cpp
```

### Comparing `pytrimal-0.5.5/CHANGELOG.md` & `pytrimal-0.6.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,26 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 
 ## [Unreleased]
-[Unreleased]: https://github.com/althonos/pytrimal/compare/v0.5.5...HEAD
+[Unreleased]: https://github.com/althonos/pytrimal/compare/v0.6.0...HEAD
+
+
+## [v0.6.0] - 2022-10-17
+[v0.6.0]: https://github.com/althonos/pytrimal/compare/v0.5.5...v0.6.0
+
+### Fixed
+- Overflow in `calculateSpuriousVector` for certain sequence block sizes.
+- MMX backend never being used unless explicitly required even when being the best supported backend.
+### Changed
+- Use `archspec` Python package instead of `cpu-features` library for CPU feature detection at runtime.
+- Use `importlib.resources.files` to load package data in `pytrimal.tests`.
 
 
 ## [v0.5.5] - 2022-10-17
 [v0.5.5]: https://github.com/althonos/pytrimal/compare/v0.5.4...v0.5.5
 
 ### Fixed
 - `calculateSpuriousVector` method of SIMD implementations not being declared `override`.
```

### Comparing `pytrimal-0.5.5/CONTRIBUTING.md` & `pytrimal-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/COPYING` & `pytrimal-0.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/MANIFEST.in` & `pytrimal-0.6.0/MANIFEST.in`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,12 @@
 recursive-include pytrimal/tests/data *
 
 recursive-include vendor/trimal         README.md LICENSE AUTHORS CHANGELOG CMakeLists.txt
 recursive-include vendor/trimal/source  *.cpp
 recursive-include vendor/trimal/include *.h *.txt
 recursive-include vendor/trimal/dataset *
 
-recursive-include vendor/cpu_features         README.md LICENSE CONTRIBUTING.md
-recursive-include vendor/cpu_features/src     *.c *.inl
-recursive-include vendor/cpu_features/include *.h
-
 recursive-include pytrimal            *.py *.pyi *.pyx *.pxd *.h py.typed
 recursive-exclude pytrimal            *.cpp *.html
 recursive-include pytrimal/patch      *.cpp *.h *.pxd
 recursive-include pytrimal/fileobj    *.cpp *.h *.pxd
 recursive-include pytrimal/impl       *.cpp *.h *.pxd
```

### Comparing `pytrimal-0.5.5/PKG-INFO` & `pytrimal-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrimal
-Version: 0.5.5
+Version: 0.6.0
 Summary: Cython bindings and Python interface to trimAl, a tool for automated alignment trimming.
 Home-page: https://github.com/althonos/pytrimal
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: GPLv3
 Project-URL: Documentation, https://pytrimal.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pytrimal/issues
@@ -22,28 +22,29 @@
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Typing :: Typed
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # 🐍✂️ PytrimAl [![Stars](https://img.shields.io/github/stars/althonos/pytrimal.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/pytrimal/stargazers)
 
 *[Cython](https://cython.org/) bindings and Python interface to [trimAl](http://trimal.cgenomics.org/), a tool for automated alignment trimming. **Now with SIMD!***
 
-[![Actions](https://img.shields.io/github/workflow/status/althonos/pytrimal/Test/main?logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/pytrimal/actions)
+[![Actions](https://img.shields.io/github/actions/workflow/status/althonos/pytrimal/test.yml?branch=main&logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/pytrimal/actions)
 [![Coverage](https://img.shields.io/codecov/c/gh/althonos/pytrimal?style=flat-square&maxAge=3600&logo=codecov)](https://codecov.io/gh/althonos/pytrimal/)
 [![License](https://img.shields.io/badge/license-GPLv3-blue.svg?style=flat-square&maxAge=2678400)](https://choosealicense.com/licenses/gpl-3.0/)
 [![PyPI](https://img.shields.io/pypi/v/pytrimal.svg?style=flat-square&maxAge=3600&logo=PyPI)](https://pypi.org/project/pytrimal)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/pytrimal?style=flat-square&maxAge=3600&logo=anaconda)](https://anaconda.org/bioconda/pytrimal)
 [![AUR](https://img.shields.io/aur/version/python-pytrimal?logo=archlinux&style=flat-square&maxAge=3600)](https://aur.archlinux.org/packages/python-pytrimal)
 [![Wheel](https://img.shields.io/pypi/wheel/pytrimal.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/pytrimal/#files)
 [![Python Versions](https://img.shields.io/pypi/pyversions/pytrimal.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/pytrimal/#files)
@@ -234,15 +235,13 @@
 
 
 ## ⚖️ License
 
 This library is provided under the [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/).
 trimAl is developed by the [trimAl team](http://trimal.cgenomics.org/trimal_team) and is distributed under the
 terms of the GPLv3 as well. See `vendor/trimal/LICENSE` for more information.
-The `cpu_features` library was written by [Guillaume Chatelet](https://github.com/gchatelet) and is
-licensed under the terms of the [Apache License 2.0](https://choosealicense.com/licenses/apache-2.0/). See `vendor/cpu_features/LICENSE` for more information.
 
 *This project is in no way not affiliated, sponsored, or otherwise endorsed
 by the [trimAl authors](http://trimal.cgenomics.org/trimal_team). It was developed
 by [Martin Larralde](https://github.com/althonos/) during his PhD project
 at the [European Molecular Biology Laboratory](https://www.embl.de/) in
 the [Zeller team](https://github.com/zellerlab).*
```

### Comparing `pytrimal-0.5.5/README.md` & `pytrimal-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # 🐍✂️ PytrimAl [![Stars](https://img.shields.io/github/stars/althonos/pytrimal.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/pytrimal/stargazers)
 
 *[Cython](https://cython.org/) bindings and Python interface to [trimAl](http://trimal.cgenomics.org/), a tool for automated alignment trimming. **Now with SIMD!***
 
-[![Actions](https://img.shields.io/github/workflow/status/althonos/pytrimal/Test/main?logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/pytrimal/actions)
+[![Actions](https://img.shields.io/github/actions/workflow/status/althonos/pytrimal/test.yml?branch=main&logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/pytrimal/actions)
 [![Coverage](https://img.shields.io/codecov/c/gh/althonos/pytrimal?style=flat-square&maxAge=3600&logo=codecov)](https://codecov.io/gh/althonos/pytrimal/)
 [![License](https://img.shields.io/badge/license-GPLv3-blue.svg?style=flat-square&maxAge=2678400)](https://choosealicense.com/licenses/gpl-3.0/)
 [![PyPI](https://img.shields.io/pypi/v/pytrimal.svg?style=flat-square&maxAge=3600&logo=PyPI)](https://pypi.org/project/pytrimal)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/pytrimal?style=flat-square&maxAge=3600&logo=anaconda)](https://anaconda.org/bioconda/pytrimal)
 [![AUR](https://img.shields.io/aur/version/python-pytrimal?logo=archlinux&style=flat-square&maxAge=3600)](https://aur.archlinux.org/packages/python-pytrimal)
 [![Wheel](https://img.shields.io/pypi/wheel/pytrimal.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/pytrimal/#files)
 [![Python Versions](https://img.shields.io/pypi/pyversions/pytrimal.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/pytrimal/#files)
@@ -197,15 +197,13 @@
 
 
 ## ⚖️ License
 
 This library is provided under the [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/).
 trimAl is developed by the [trimAl team](http://trimal.cgenomics.org/trimal_team) and is distributed under the
 terms of the GPLv3 as well. See `vendor/trimal/LICENSE` for more information.
-The `cpu_features` library was written by [Guillaume Chatelet](https://github.com/gchatelet) and is
-licensed under the terms of the [Apache License 2.0](https://choosealicense.com/licenses/apache-2.0/). See `vendor/cpu_features/LICENSE` for more information.
 
 *This project is in no way not affiliated, sponsored, or otherwise endorsed
 by the [trimAl authors](http://trimal.cgenomics.org/trimal_team). It was developed
 by [Martin Larralde](https://github.com/althonos/) during his PhD project
 at the [European Molecular Biology Laboratory](https://www.embl.de/) in
 the [Zeller team](https://github.com/zellerlab).*
```

### Comparing `pytrimal-0.5.5/include/_unicode.pxd` & `pytrimal-0.6.0/include/_unicode.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/include/cpu_features/aarch64.pxd` & `pytrimal-0.6.0/include/cpu_features/aarch64.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/include/cpu_features/arm.pxd` & `pytrimal-0.6.0/include/cpu_features/arm.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/include/cpu_features/x86.pxd` & `pytrimal-0.6.0/include/cpu_features/x86.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/include/iostream.pxd` & `pytrimal-0.6.0/include/iostream.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/include/trimal/alignment.pxd` & `pytrimal-0.6.0/include/trimal/alignment.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/include/trimal/cleaner.pxd` & `pytrimal-0.6.0/include/trimal/cleaner.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/include/trimal/format_handling.pxd` & `pytrimal-0.6.0/include/trimal/format_handling.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/include/trimal/manager.pxd` & `pytrimal-0.6.0/include/trimal/manager.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/include/trimal/report_system.pxd` & `pytrimal-0.6.0/include/trimal/report_system.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/include/trimal/statistics.pxd` & `pytrimal-0.6.0/include/trimal/statistics.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/patches/clustal_state.cpp.patch` & `pytrimal-0.6.0/patches/clustal_state.cpp.patch`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/patches/fasta_state.cpp.patch` & `pytrimal-0.6.0/patches/fasta_state.cpp.patch`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/patches/nexus_state.cpp.patch` & `pytrimal-0.6.0/patches/nexus_state.cpp.patch`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/patches/phylip32_state.cpp.patch` & `pytrimal-0.6.0/patches/phylip32_state.cpp.patch`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/patches/phylip40_state.cpp.patch` & `pytrimal-0.6.0/patches/phylip40_state.cpp.patch`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/patches/pir_state.cpp.patch` & `pytrimal-0.6.0/patches/pir_state.cpp.patch`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/__init__.py` & `pytrimal-0.6.0/pytrimal/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/_trimal.pxd` & `pytrimal-0.6.0/pytrimal/_trimal.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/_trimal.pyi` & `pytrimal-0.6.0/pytrimal/_trimal.pyi`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/_trimal.pyx` & `pytrimal-0.6.0/pytrimal/_trimal.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -50,67 +50,83 @@
 IF MMX_BUILD_SUPPORT:
     from pytrimal.impl.mmx cimport MMXSimilarity, MMXGaps, MMXCleaner
 IF NEON_BUILD_SUPPORT:
     from pytrimal.impl.neon cimport NEONSimilarity, NEONGaps, NEONCleaner
 IF AVX2_BUILD_SUPPORT:
     from pytrimal.impl.avx cimport AVXSimilarity, AVXGaps, AVXCleaner
 
+
 # --- Python imports ---------------------------------------------------------
 
 import os
 import threading
 
+import archspec.cpu
+
+include "_version.py"
+
+
+# --- Patch for PyPy 3.9 -----------------------------------------------------
+
+IF not HAS_PYINTERPRETERSTATE_GETID:
+    cdef extern from *:
+        """
+        int64_t PyInterpreterState_GetID(PyInterpreterState *interp) {
+            return 0;
+        }
+        """
+
+
 # --- Constants --------------------------------------------------------------
 
 _TARGET_CPU           = TARGET_CPU
+_HOST_CPU             = archspec.cpu.host()
 _SSE2_BUILD_SUPPORT   = False
 _SSE2_RUNTIME_SUPPORT = False
 _MMX_BUILD_SUPPORT    = False
 _MMX_RUNTIME_SUPPORT  = False
 _AVX2_BUILD_SUPPORT   = False
 _AVX2_RUNTIME_SUPPORT = False
 _NEON_BUILD_SUPPORT   = False
 _NEON_RUNTIME_SUPPORT = False
 
 IF TARGET_CPU == "x86" and TARGET_SYSTEM in ("freebsd", "linux_or_android", "macos", "windows"):
-    from cpu_features.x86 cimport GetX86Info, X86Info
-    cdef X86Info cpu_info = GetX86Info()
     _MMX_BUILD_SUPPORT    = MMX_BUILD_SUPPORT
-    _MMX_RUNTIME_SUPPORT  = MMX_BUILD_SUPPORT  and cpu_info.features.mmx != 0
     _SSE2_BUILD_SUPPORT   = SSE2_BUILD_SUPPORT
-    _SSE2_RUNTIME_SUPPORT = SSE2_BUILD_SUPPORT and cpu_info.features.sse2 != 0
     _AVX2_BUILD_SUPPORT   = AVX2_BUILD_SUPPORT
-    _AVX2_RUNTIME_SUPPORT = AVX2_BUILD_SUPPORT and cpu_info.features.avx2 != 0
-ELIF TARGET_CPU == "arm":
-    from cpu_features.arm cimport GetArmInfo, ArmInfo
-    cdef ArmInfo arm_info = GetArmInfo()
+    _MMX_RUNTIME_SUPPORT  = "mmx" in _HOST_CPU.features
+    _SSE2_RUNTIME_SUPPORT = "sse2" in _HOST_CPU.features
+    _AVX2_RUNTIME_SUPPORT = "avx2" in _HOST_CPU.features
+ELIF TARGET_CPU == "arm" and TARGET_SYSTEM == "linux_or_android":
     _NEON_BUILD_SUPPORT   = NEON_BUILD_SUPPORT
-    _NEON_RUNTIME_SUPPORT = NEON_BUILD_SUPPORT and arm_info.features.neon != 0
+    _NEON_RUNTIME_SUPPORT = "neon" in _HOST_CPU.features
 ELIF TARGET_CPU == "aarch64":
     _NEON_BUILD_SUPPORT   = NEON_BUILD_SUPPORT
-    _NEON_RUNTIME_SUPPORT = NEON_BUILD_SUPPORT # always runtime support on Aarch64
-
+    _NEON_RUNTIME_SUPPORT = NEON_BUILD_SUPPORT  # always runtime support on Aarch64
 
 if _AVX2_RUNTIME_SUPPORT:
     _BEST_BACKEND = simd_backend.AVX2
 elif _SSE2_RUNTIME_SUPPORT:
     _BEST_BACKEND = simd_backend.SSE2
+elif _MMX_RUNTIME_SUPPORT:
+    _BEST_BACKEND = simd_backend.MMX
 elif _NEON_RUNTIME_SUPPORT:
     _BEST_BACKEND = simd_backend.NEON
 else:
     _BEST_BACKEND = simd_backend.GENERIC
 
 cdef enum simd_backend:
     NONE = 0
     GENERIC = 1
     SSE2 = 2
     NEON = 3
     AVX2 = 4
     MMX = 5
 
+
 # --- Utilities --------------------------------------------------------------
 
 ctypedef fused number:
     int
     float
     ssize_t
 
@@ -1837,15 +1853,14 @@
         manager.automatedMethodCount  = 0
         manager.clusters              = self._clusters
         manager.maxIdentity           = self._identity_threshold
 
 
 # -- Misc classes ------------------------------------------------------------
 
-
 cdef class SimilarityMatrix:
     """A similarity matrix for biological sequence characters.
     """
 
     # --- Class methods ------------------------------------------------------
 
     @classmethod
```

### Comparing `pytrimal-0.5.5/pytrimal/fileobj/pyreadbuf.cpp` & `pytrimal-0.6.0/pytrimal/fileobj/pyreadbuf.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/fileobj/pyreadbuf.h` & `pytrimal-0.6.0/pytrimal/fileobj/pyreadbuf.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/fileobj/pyreadintobuf.cpp` & `pytrimal-0.6.0/pytrimal/fileobj/pyreadintobuf.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/fileobj/pyreadintobuf.h` & `pytrimal-0.6.0/pytrimal/fileobj/pyreadintobuf.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/fileobj/pywritebuf.cpp` & `pytrimal-0.6.0/pytrimal/fileobj/pywritebuf.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/impl/avx.cpp` & `pytrimal-0.6.0/pytrimal/impl/avx.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/impl/avx.h` & `pytrimal-0.6.0/pytrimal/impl/avx.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/impl/generic.cpp` & `pytrimal-0.6.0/pytrimal/impl/generic.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/impl/generic.h` & `pytrimal-0.6.0/pytrimal/impl/generic.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/impl/generic.pxd` & `pytrimal-0.6.0/pytrimal/impl/generic.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/impl/mmx.cpp` & `pytrimal-0.6.0/pytrimal/impl/mmx.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/impl/mmx.h` & `pytrimal-0.6.0/pytrimal/impl/mmx.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/impl/neon.cpp` & `pytrimal-0.6.0/pytrimal/impl/neon.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/impl/neon.h` & `pytrimal-0.6.0/pytrimal/impl/neon.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/impl/sse.cpp` & `pytrimal-0.6.0/pytrimal/impl/sse.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/impl/sse.h` & `pytrimal-0.6.0/pytrimal/impl/sse.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/impl/template.h` & `pytrimal-0.6.0/pytrimal/impl/template.h`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
     memset(&hits[0], 0, c.alig->originalNumberOfResidues * sizeof(uint32_t));
     memset(&hits_u8[0], 0, c.alig->originalNumberOfResidues * sizeof(uint8_t));
 
     const uint8_t *datai =
         reinterpret_cast<const uint8_t *>(c.alig->sequences[i].data());
 
     // compare sequence to other sequences for every position
+    unsigned int processedSequences = 0;
     for (int j = 0; j < c.alig->originalNumberOfSequences; j++) {
 
       // don't compare sequence to itself
       if (j == i)
         continue;
 
       const uint8_t *dataj =
@@ -204,15 +205,16 @@
         int nongapj = (dataj[k] != indet) && (dataj[k] != '-');
         hits_u8[k] += ((nongapi && nongapj) || (datai[k] == dataj[k]));
       }
 
       // we can process up to UCHAR_MAX sequences, otherwise hits_u8[k]
       // may overflow, so every UCHAR_MAX iterations we transfer the
       // partial hit counts from `hits_u8` to `hits`
-      if ((j % UCHAR_MAX) == 0) {
+      processedSequences++;
+      if ((processedSequences % UCHAR_MAX) == 0) {
         for (k = 0; k < c.alig->originalNumberOfResidues; k++)
           hits[k] += hits_u8[k];
         memset(hits_u8, 0, c.alig->originalNumberOfResidues * sizeof(uint8_t));
       }
     }
 
     // update counters after last loop
@@ -553,8 +555,8 @@
   for (int i = 0; i < s.alig->originalNumberOfSequences; i++)
     delete[] s.matrixIdentity[i];
   delete[] s.matrixIdentity;
   s.matrixIdentity = nullptr;
 
   return true;
 }
-} // namespace simd
+} // namespace simd
```

### Comparing `pytrimal-0.5.5/pytrimal/patch/reportsystem.cpp` & `pytrimal-0.6.0/pytrimal/patch/reportsystem.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/__init__.py` & `pytrimal-0.6.0/pytrimal/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.automated1.fasta` & `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.automated1.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.clusters10.fasta` & `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.clusters10.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.clusters5.fasta` & `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.clusters5.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.cons40.gt40.fasta` & `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.cons40.gt40.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.cons60.gt90.fasta` & `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.cons60.gt90.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.fasta` & `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.gappyout.fasta` & `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.gappyout.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.id50.fasta` & `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.id50.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.id70.fasta` & `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.id70.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.maxidentity75.fasta` & `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.maxidentity75.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.noallgaps.fasta` & `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.noallgaps.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.noduplicateseqs.fasta` & `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.noduplicateseqs.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.seq40.res60.fasta` & `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.seq40.res60.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.seq80.res80.fasta` & `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.seq80.res80.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.strict.fasta` & `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.strict.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/ENOG411BWBU.strictplus.fasta` & `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.strictplus.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/PF12574.full.afa` & `pytrimal-0.6.0/pytrimal/tests/data/PF12574.full.afa`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/halorhodopsin.afa` & `pytrimal-0.6.0/pytrimal/tests/data/halorhodopsin.afa`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/data/pam70.json` & `pytrimal-0.6.0/pytrimal/tests/data/pam70.json`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/test_alignment.py` & `pytrimal-0.6.0/pytrimal/tests/test_alignment.py`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/test_automatic_trimmer.py` & `pytrimal-0.6.0/pytrimal/tests/test_automatic_trimmer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,18 @@
 import os
 import pickle
 import sys
 import json
 import unittest
 
-try:
-    try:
-        import importlib.resources as importlib_resources
-    except ImportError:
-        import importlib_resources
-except ImportError:
-    importlib_resources = None
-
 from .. import _trimal, Alignment, AutomaticTrimmer, SimilarityMatrix
+from ._base import TrimmerTestCase, files
 
 
-class TestAutomaticTrimmer(unittest.TestCase):
-    backend = None
-
-    def assertTrimmedAlignmentEqual(self, trimmed, expected):
-        self.assertEqual(len(trimmed.names), len(expected.names))
-        self.assertEqual(len(trimmed.sequences), len(expected.sequences))
-        self.assertEqual(trimmed.names, expected.names)
-        for seq1, seq2 in zip(trimmed.sequences, expected.sequences):
-            self.assertEqual(seq1, seq2)
-
-    @staticmethod
-    def _load_alignment(name):
-        with importlib_resources.path("pytrimal.tests.data", name) as path:
-            return Alignment.load(path)
+class TestAutomaticTrimmer(TrimmerTestCase, unittest.TestCase):
 
     def _test_method(self, name):
         ali = self._load_alignment("ENOG411BWBU.fasta")
         expected = self._load_alignment("ENOG411BWBU.{}.fasta".format(name))
         trimmer = AutomaticTrimmer(method=name, backend=self.backend)
         trimmed = trimmer.trim(ali)
         self.assertTrimmedAlignmentEqual(trimmed, expected)
@@ -48,48 +28,48 @@
         self.assertEqual(repr(trimmer), "AutomaticTrimmer('automated1')")
         trimmer = AutomaticTrimmer("noduplicateseqs", backend=None)
         self.assertEqual(
             repr(trimmer), "AutomaticTrimmer('noduplicateseqs', backend=None)"
         )
 
     @unittest.skipIf(sys.version_info < (3, 6), "No pathlib support in Python 3.5")
-    @unittest.skipUnless(importlib_resources, "importlib.resources not available")
+    @unittest.skipUnless(files, "importlib.resources.files not available")
     def test_strict_method(self):
         self._test_method("strict")
 
     @unittest.skipIf(sys.version_info < (3, 6), "No pathlib support in Python 3.5")
-    @unittest.skipUnless(importlib_resources, "importlib.resources not available")
+    @unittest.skipUnless(files, "importlib.resources.files not available")
     def test_strictplus_method(self):
         self._test_method("strictplus")
 
     @unittest.skipIf(sys.version_info < (3, 6), "No pathlib support in Python 3.5")
-    @unittest.skipUnless(importlib_resources, "importlib.resources not available")
+    @unittest.skipUnless(files, "importlib.resources.files not available")
     def test_automatic1_method(self):
         self._test_method("automated1")
 
     @unittest.skipIf(sys.version_info < (3, 6), "No pathlib support in Python 3.5")
-    @unittest.skipUnless(importlib_resources, "importlib.resources not available")
+    @unittest.skipUnless(files, "importlib.resources.files not available")
     def test_noallgaps_method(self):
         self._test_method("noallgaps")
 
     @unittest.skipIf(sys.version_info < (3, 6), "No pathlib support in Python 3.5")
-    @unittest.skipUnless(importlib_resources, "importlib.resources not available")
+    @unittest.skipUnless(files, "importlib.resources.files not available")
     def test_gappyout_method(self):
         self._test_method("gappyout")
 
     @unittest.skipIf(sys.version_info < (3, 6), "No pathlib support in Python 3.5")
-    @unittest.skipUnless(importlib_resources, "importlib.resources not available")
+    @unittest.skipUnless(files, "importlib.resources.files not available")
     def test_noduplicateseqs_method(self):
         self._test_method("noduplicateseqs")
 
     @unittest.skipIf(sys.version_info < (3, 6), "No pathlib support in Python 3.5")
-    @unittest.skipUnless(importlib_resources, "importlib.resources not available")
+    @unittest.skipUnless(files, "importlib.resources.files not available")
     def test_custom_similarity_matrix(self):
         alignment = self._load_alignment("ENOG411BWBU.fasta")
-        with importlib_resources.open_binary("pytrimal.tests.data", "pam70.json") as f:
+        with self._open_data("pam70.json", "rb") as f:
             pam70 = SimilarityMatrix(**json.load(f))
 
         trimmer = AutomaticTrimmer("strict", backend=self.backend)
         trimmed = trimmer.trim(alignment, pam70)
 
     def test_invalid_characters(self):
         alignment = Alignment([b"seq1", b"seq2"], ["MKKBO", "MKKAY"])
```

### Comparing `pytrimal-0.5.5/pytrimal/tests/test_doctest.py` & `pytrimal-0.6.0/pytrimal/tests/test_doctest.py`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/test_manual_trimmer.py` & `pytrimal-0.6.0/pytrimal/tests/test_manual_trimmer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,17 @@
 import os
 import pickle
 import sys
 import unittest
 
-try:
-    try:
-        import importlib.resources as importlib_resources
-    except ImportError:
-        import importlib_resources
-except ImportError:
-    importlib_resources = None
-
 from .. import _trimal, Alignment, ManualTrimmer
+from ._base import TrimmerTestCase, files
 
 
-class TestManualTrimmer(unittest.TestCase):
-    backend = None
-
-    def assertTrimmedAlignmentEqual(self, trimmed, expected):
-        self.assertEqual(len(trimmed.names), len(expected.names))
-        self.assertEqual(len(trimmed.sequences), len(expected.sequences))
-        self.assertEqual(trimmed.names, expected.names)
-        for seq1, seq2 in zip(trimmed.sequences, expected.sequences):
-            self.assertEqual(seq1, seq2)
-
-    @staticmethod
-    def _load_alignment(name):
-        with importlib_resources.path("pytrimal.tests.data", name) as path:
-            return Alignment.load(path)
+class TestManualTrimmer(TrimmerTestCase, unittest.TestCase):
 
     def _test_parameters(self, gt, cons):
         ali = self._load_alignment("ENOG411BWBU.fasta")
         filename = "ENOG411BWBU.cons{:02}.gt{:02}.fasta".format(cons, int(gt * 100))
         expected = self._load_alignment(filename)
         trimmer = ManualTrimmer(gap_threshold=gt, conservation_percentage=cons, backend=self.backend)
         trimmed = trimmer.trim(ali)
@@ -45,24 +25,24 @@
         self.assertRaises(ValueError, ManualTrimmer, conservation_percentage=-2)
         self.assertRaises(
             ValueError, ManualTrimmer, gap_threshold=0.5, gap_absolute_threshold=0.5
         )
         self.assertRaises(ValueError, ManualTrimmer, window=5, gap_window=5)
 
     @unittest.skipIf(sys.version_info < (3, 6), "No pathlib support in Python 3.5")
-    @unittest.skipUnless(importlib_resources, "importlib.resources not available")
+    @unittest.skipUnless(files, "importlib.resources.files not available")
     def test_gap_threshold(self):
         self._test_parameters(gt=0.9, cons=60)
         self._test_parameters(gt=0.4, cons=40)
 
     @unittest.skipIf(sys.version_info < (3, 6), "No pathlib support in Python 3.5")
-    @unittest.skipUnless(importlib_resources, "importlib.resources not available")
+    @unittest.skipUnless(files, "importlib.resources.files not available")
     def test_window(self):
-        ali = self._load_alignment("example.001.AA.clw")
-        expected = self._load_alignment("example.001.gt90.w3.fasta")
+        ali = self._load_alignment("example.001.AA.clw", "clustal")
+        expected = self._load_alignment("example.001.gt90.w3.clw", "clustal")
 
         trimmer = ManualTrimmer(gap_threshold=0.9, window=3, backend=self.backend)
         trimmed = trimmer.trim(ali)
 
         self.assertEqual(trimmed.names, expected.names)
         for seq1, seq2 in zip(trimmed.sequences, expected.sequences):
             self.assertEqual(seq1, seq2)
```

### Comparing `pytrimal-0.5.5/pytrimal/tests/test_overlap_trimmer.py` & `pytrimal-0.6.0/pytrimal/tests/test_overlap_trimmer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,35 @@
 import os
 import sys
 import json
 import pickle
 import unittest
 
-try:
-    try:
-        import importlib.resources as importlib_resources
-    except ImportError:
-        import importlib_resources
-except ImportError:
-    importlib_resources = None
-
 from .. import _trimal, Alignment, OverlapTrimmer
+from ._base import TrimmerTestCase, files
 
 
-class TestOverlapTrimmer(unittest.TestCase):
-    backend = None
-
-    def assertTrimmedAlignmentEqual(self, trimmed, expected):
-        self.assertEqual(len(trimmed.names), len(expected.names))
-        self.assertEqual(len(trimmed.sequences), len(expected.sequences))
-        self.assertEqual(trimmed.names, expected.names)
-        for seq1, seq2 in zip(trimmed.sequences, expected.sequences):
-            self.assertEqual(seq1, seq2)
-
-    @staticmethod
-    def _load_alignment(name):
-        with importlib_resources.path("pytrimal.tests.data", name) as path:
-            return Alignment.load(path)
+class TestOverlapTrimmer(TrimmerTestCase, unittest.TestCase):
 
     def _test_overlap(self, seq, res):
         ali = self._load_alignment("ENOG411BWBU.fasta")
         expected = self._load_alignment(
             "ENOG411BWBU.seq{}.res{}.fasta".format(seq, res)
         )
         trimmer = OverlapTrimmer(sequence_overlap=seq, residue_overlap=res / 100, backend=self.backend)
         trimmed = trimmer.trim(ali)
         self.assertTrimmedAlignmentEqual(trimmed, expected)
 
     @unittest.skipIf(sys.version_info < (3, 6), "No pathlib support in Python 3.5")
-    @unittest.skipUnless(importlib_resources, "importlib.resources not available")
+    @unittest.skipUnless(files, "importlib.resources.files not available")
     def test_seqoverlap80_resoverlap80(self):
         self._test_overlap(80, 80)
 
     @unittest.skipIf(sys.version_info < (3, 6), "No pathlib support in Python 3.5")
-    @unittest.skipUnless(importlib_resources, "importlib.resources not available")
+    @unittest.skipUnless(files, "importlib.resources.files not available")
     def test_seqoverlap40_resoverlap60(self):
         self._test_overlap(40, 60)
 
     def test_repr(self):
         trimmer = OverlapTrimmer(80, 0.5)
         self.assertEqual(repr(trimmer), "OverlapTrimmer(80.0, 0.5)")
         trimmer = OverlapTrimmer(50, 1.0)
```

### Comparing `pytrimal-0.5.5/pytrimal/tests/test_representative_trimmer.py` & `pytrimal-0.6.0/pytrimal/tests/test_representative_trimmer.py`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal/tests/test_similarity_matrix.py` & `pytrimal-0.6.0/pytrimal/tests/test_similarity_matrix.py`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/pytrimal.egg-info/PKG-INFO` & `pytrimal-0.6.0/pytrimal.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrimal
-Version: 0.5.5
+Version: 0.6.0
 Summary: Cython bindings and Python interface to trimAl, a tool for automated alignment trimming.
 Home-page: https://github.com/althonos/pytrimal
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: GPLv3
 Project-URL: Documentation, https://pytrimal.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pytrimal/issues
@@ -22,28 +22,29 @@
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Typing :: Typed
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # 🐍✂️ PytrimAl [![Stars](https://img.shields.io/github/stars/althonos/pytrimal.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/pytrimal/stargazers)
 
 *[Cython](https://cython.org/) bindings and Python interface to [trimAl](http://trimal.cgenomics.org/), a tool for automated alignment trimming. **Now with SIMD!***
 
-[![Actions](https://img.shields.io/github/workflow/status/althonos/pytrimal/Test/main?logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/pytrimal/actions)
+[![Actions](https://img.shields.io/github/actions/workflow/status/althonos/pytrimal/test.yml?branch=main&logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/pytrimal/actions)
 [![Coverage](https://img.shields.io/codecov/c/gh/althonos/pytrimal?style=flat-square&maxAge=3600&logo=codecov)](https://codecov.io/gh/althonos/pytrimal/)
 [![License](https://img.shields.io/badge/license-GPLv3-blue.svg?style=flat-square&maxAge=2678400)](https://choosealicense.com/licenses/gpl-3.0/)
 [![PyPI](https://img.shields.io/pypi/v/pytrimal.svg?style=flat-square&maxAge=3600&logo=PyPI)](https://pypi.org/project/pytrimal)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/pytrimal?style=flat-square&maxAge=3600&logo=anaconda)](https://anaconda.org/bioconda/pytrimal)
 [![AUR](https://img.shields.io/aur/version/python-pytrimal?logo=archlinux&style=flat-square&maxAge=3600)](https://aur.archlinux.org/packages/python-pytrimal)
 [![Wheel](https://img.shields.io/pypi/wheel/pytrimal.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/pytrimal/#files)
 [![Python Versions](https://img.shields.io/pypi/pyversions/pytrimal.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/pytrimal/#files)
@@ -234,15 +235,13 @@
 
 
 ## ⚖️ License
 
 This library is provided under the [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/).
 trimAl is developed by the [trimAl team](http://trimal.cgenomics.org/trimal_team) and is distributed under the
 terms of the GPLv3 as well. See `vendor/trimal/LICENSE` for more information.
-The `cpu_features` library was written by [Guillaume Chatelet](https://github.com/gchatelet) and is
-licensed under the terms of the [Apache License 2.0](https://choosealicense.com/licenses/apache-2.0/). See `vendor/cpu_features/LICENSE` for more information.
 
 *This project is in no way not affiliated, sponsored, or otherwise endorsed
 by the [trimAl authors](http://trimal.cgenomics.org/trimal_team). It was developed
 by [Martin Larralde](https://github.com/althonos/) during his PhD project
 at the [European Molecular Biology Laboratory](https://www.embl.de/) in
 the [Zeller team](https://github.com/zellerlab).*
```

### Comparing `pytrimal-0.5.5/pytrimal.egg-info/SOURCES.txt` & `pytrimal-0.6.0/pytrimal.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 pytrimal/_trimal.pyx
 pytrimal/_version.py
 pytrimal/py.typed
 pytrimal.egg-info/PKG-INFO
 pytrimal.egg-info/SOURCES.txt
 pytrimal.egg-info/dependency_links.txt
 pytrimal.egg-info/not-zip-safe
+pytrimal.egg-info/requires.txt
 pytrimal.egg-info/top_level.txt
 pytrimal/fileobj/__init__.pxd
 pytrimal/fileobj/pyreadbuf.cpp
 pytrimal/fileobj/pyreadbuf.h
 pytrimal/fileobj/pyreadintobuf.cpp
 pytrimal/fileobj/pyreadintobuf.h
 pytrimal/fileobj/pywritebuf.cpp
@@ -93,14 +94,15 @@
 pytrimal/impl/sse.h
 pytrimal/impl/sse.pxd
 pytrimal/impl/template.h
 pytrimal/patch/omp.h
 pytrimal/patch/reportsystem.cpp
 pytrimal/tests/__init__.py
 pytrimal/tests/__main__.py
+pytrimal/tests/_base.py
 pytrimal/tests/requirements.txt
 pytrimal/tests/test_alignment.py
 pytrimal/tests/test_automatic_trimmer.py
 pytrimal/tests/test_doctest.py
 pytrimal/tests/test_manual_trimmer.py
 pytrimal/tests/test_overlap_trimmer.py
 pytrimal/tests/test_representative_trimmer.py
@@ -120,54 +122,17 @@
 pytrimal/tests/data/ENOG411BWBU.seq40.res60.fasta
 pytrimal/tests/data/ENOG411BWBU.seq80.res80.fasta
 pytrimal/tests/data/ENOG411BWBU.strict.fasta
 pytrimal/tests/data/ENOG411BWBU.strictplus.fasta
 pytrimal/tests/data/PF12574.full.afa
 pytrimal/tests/data/__init__.py
 pytrimal/tests/data/example.001.AA.clw
-pytrimal/tests/data/example.001.gt90.w3.fasta
+pytrimal/tests/data/example.001.gt90.w3.clw
 pytrimal/tests/data/halorhodopsin.afa
 pytrimal/tests/data/pam70.json
-vendor/cpu_features/CONTRIBUTING.md
-vendor/cpu_features/LICENSE
-vendor/cpu_features/README.md
-vendor/cpu_features/ci/README.md
-vendor/cpu_features/cmake/README.md
-vendor/cpu_features/include/cpu_features_cache_info.h
-vendor/cpu_features/include/cpu_features_macros.h
-vendor/cpu_features/include/cpuinfo_aarch64.h
-vendor/cpu_features/include/cpuinfo_arm.h
-vendor/cpu_features/include/cpuinfo_mips.h
-vendor/cpu_features/include/cpuinfo_ppc.h
-vendor/cpu_features/include/cpuinfo_x86.h
-vendor/cpu_features/include/internal/bit_utils.h
-vendor/cpu_features/include/internal/cpuid_x86.h
-vendor/cpu_features/include/internal/filesystem.h
-vendor/cpu_features/include/internal/hwcaps.h
-vendor/cpu_features/include/internal/stack_line_reader.h
-vendor/cpu_features/include/internal/string_view.h
-vendor/cpu_features/ndk_compat/README.md
-vendor/cpu_features/src/copy.inl
-vendor/cpu_features/src/define_introspection.inl
-vendor/cpu_features/src/define_introspection_and_hwcaps.inl
-vendor/cpu_features/src/equals.inl
-vendor/cpu_features/src/filesystem.c
-vendor/cpu_features/src/hwcaps.c
-vendor/cpu_features/src/impl_aarch64_linux_or_android.c
-vendor/cpu_features/src/impl_arm_linux_or_android.c
-vendor/cpu_features/src/impl_mips_linux_or_android.c
-vendor/cpu_features/src/impl_ppc_linux.c
-vendor/cpu_features/src/impl_x86__base_implementation.inl
-vendor/cpu_features/src/impl_x86_freebsd.c
-vendor/cpu_features/src/impl_x86_linux_or_android.c
-vendor/cpu_features/src/impl_x86_macos.c
-vendor/cpu_features/src/impl_x86_windows.c
-vendor/cpu_features/src/stack_line_reader.c
-vendor/cpu_features/src/string_view.c
-vendor/cpu_features/src/utils/list_cpu_features.c
 vendor/trimal/AUTHORS
 vendor/trimal/CHANGELOG
 vendor/trimal/CMakeLists.txt
 vendor/trimal/LICENSE
 vendor/trimal/README.md
 vendor/trimal/dataset/alignments_comparison.1
 vendor/trimal/dataset/alignments_comparison.2
```

### Comparing `pytrimal-0.5.5/setup.cfg` & `pytrimal-0.6.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 	Programming Language :: C
 	Programming Language :: Cython
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	Topic :: Scientific/Engineering :: Medical Science Apps.
 	Typing :: Typed
 project_urls = 
 	Documentation = https://pytrimal.readthedocs.io/en/stable/
@@ -40,16 +41,18 @@
 zip_safe = false
 packages = pytrimal, pytrimal.tests, pytrimal.tests.data
 include_package_data = false
 python_requires = >=3.5
 setup_requires = 
 	setuptools >=46.4
 	cython ~=0.29.16
+install_requires = 
+	archspec ~=0.1
 tests_require = 
-	importlib-resources ; python_version < '3.7'
+	importlib-resources ; python_version < '3.9'
 
 [options.package_data]
 pytrimal = py.typed, *.pyi
 pytrimal.tests = requirements.txt
 pytrimal.tests.data = *
 
 [coverage:run]
```

### Comparing `pytrimal-0.5.5/setup.py` & `pytrimal-0.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -311,14 +311,53 @@
                               a = vabsq_s16(a);
                     short     x = vgetq_lane_s16(a, 1);
                     return (x == 1) ? 0 : 1;
                 }}
             """,
         )
 
+    def _check_getid(self):
+        _eprint('checking whether `PyInterpreterState_GetID` is available')
+
+        base = "have_getid"
+        testfile = os.path.join(self.build_temp, "{}.c".format(base))
+        objects = []
+
+        self.mkpath(self.build_temp)
+        with open(testfile, "w") as f:
+            f.write("""
+            #include <stdint.h>
+            #include <stdlib.h>
+            #include <Python.h>
+
+            int main(int argc, char *argv[]) {{
+                PyInterpreterState_GetID(NULL);
+                return 0;
+            }}
+            """)
+
+        if self.compiler.compiler_type == "msvc":
+            flags = ["/WX"]
+        else:
+            flags = ["-Werror=implicit-function-declaration"]
+
+        try:
+            self.mkpath(self.build_temp)
+            objects = self.compiler.compile([testfile], extra_postargs=flags)
+        except CompileError:
+            _eprint("no")
+            return False
+        else:
+            _eprint("yes")
+            return True
+        finally:
+            os.remove(testfile)
+            for obj in filter(os.path.isfile, objects):
+                os.remove(obj)
+
     # --- Build code ---
 
     def build_simd_code(self, ext):
         # build platform-specific code
         for simd, sources in ext.platform_sources.items():
             if self._simd_supported[simd] and not self._simd_disabled[simd]:
                 objects = [
@@ -403,14 +442,15 @@
         cython_args = {
             "include_path": ["include"],
             "compiler_directives": {
                 "cdivision": True,
                 "nonecheck": False,
             },
             "compile_time_env": {
+                "HAS_PYINTERPRETERSTATE_GETID": self._check_getid(),
                 "SYS_IMPLEMENTATION_NAME": sys.implementation.name,
                 "SYS_VERSION_INFO_MAJOR": sys.version_info.major,
                 "SYS_VERSION_INFO_MINOR": sys.version_info.minor,
                 "SYS_VERSION_INFO_MICRO": sys.version_info.micro,
                 "DEFAULT_BUFFER_SIZE": io.DEFAULT_BUFFER_SIZE,
                 "TARGET_CPU": TARGET_CPU,
                 "TARGET_SYSTEM": TARGET_SYSTEM,
@@ -572,47 +612,28 @@
 
     def get_library(self, name):
         return next(lib for lib in self.libraries if lib.name == name)
 
     # --- Build code ---
 
     def build_libraries(self, libraries):
-        # check for functions required for libcpu_features on OSX
-        if SYSTEM == "Darwin":
-            _patch_osx_compiler(self.compiler)
-            if self._check_function(
-                "sysctlbyname", "sys/sysctl.h", args="(NULL, NULL, 0, NULL, 0)"
-            ):
-                self.compiler.define_macro("HAVE_SYSCTLBYNAME", 1)
-
         # build each library only if the sources are outdated
         self.mkpath(self.build_clib)
         for library in libraries:
             libname = self.compiler.library_filename(
                 library.name, output_dir=self.build_clib
             )
             self.make_file(library.sources, libname, self.build_library, (library,))
 
     def build_library(self, library):
         # show the compiler being used
         _eprint(
             "building", library.name, "with", self.compiler.compiler_type, "compiler"
         )
 
-        # detect hardware detection capabilities of CPU features
-        hwcaps = False
-        if self._check_function("getauxval", "sys/auxv.h", "(0)"):
-            library.define_macros.append(("HAVE_STRONG_GETAUXVAL", 1))
-            hwcaps = True
-        if self._check_function("dlclose", "dlfcn.h", "(0)"):
-            library.define_macros.append(("HAVE_DLFCN_H", 1))
-            hwcaps = True
-        if library.name == "cpu_features" and hwcaps and TARGET_SYSTEM in ("linux_or_android", "freebsd", "macos"):
-            library.sources.append(os.path.join("vendor", "cpu_features", "src", "hwcaps.c"))
-
         # add debug flags if we are building in debug mode
         if self.debug:
             if self.compiler.compiler_type in {"unix", "cygwin", "mingw32"}:
                 library.extra_compile_args.append("-g")
             elif self.compiler.compiler_type == "msvc":
                 library.extra_compile_args.append("/Z7")
 
@@ -686,15 +707,15 @@
 
 
 class clean(_clean):
     """A `clean` that removes intermediate files created by Cython."""
 
     def run(self):
 
-        source_dir = os.path.join(os.path.dirname(__file__), "pymuscle5")
+        source_dir = os.path.join(os.path.dirname(__file__), "pytrimal")
 
         patterns = ["*.html"]
         if self.all:
             patterns.extend(["*.so", "*.c", "*.cpp"])
 
         for pattern in patterns:
             for file in glob.glob(os.path.join(source_dir, pattern)):
@@ -778,37 +799,16 @@
     include_dirs=[
         os.path.join("pytrimal", "patch"),
         "pytrimal",
         "include",
     ],
 )
 
-CPU_FEATURES = Library(
-    "cpu_features",
-    language="c",
-    sources=[
-        os.path.join("vendor", "cpu_features", "src", base)
-        for base in [
-            "impl_{}_{}.c".format(TARGET_CPU, TARGET_SYSTEM),
-            "filesystem.c",
-            "stack_line_reader.c",
-            "string_view.c",
-            "copy.inl",
-            "define_introspection.inl",
-            "define_introspection_and_hwcaps.inl",
-            "equals.inl",
-            "impl_x86__base_implementation.inl",
-        ]
-    ],
-    include_dirs=[os.path.join("vendor", "cpu_features", "include")],
-    define_macros=[("STACK_LINE_READER_BUFFER_SIZE", 1024)],
-)
-
 setuptools.setup(
-    libraries=[CPU_FEATURES, TRIMAL],
+    libraries=[TRIMAL],
     ext_modules=[
         Extension(
             "pytrimal._trimal",
             language="c++",
             sources=[
                 os.path.join("pytrimal", "fileobj", "pywritebuf.cpp"),
                 os.path.join("pytrimal", "fileobj", "pyreadbuf.cpp"),
@@ -823,20 +823,18 @@
                 "AVX2": [os.path.join("pytrimal", "impl", "avx.cpp")],
                 "MMX": [os.path.join("pytrimal", "impl", "mmx.cpp")],
             },
             include_dirs=[
                 os.path.join("pytrimal", "patch"),
                 os.path.join("pytrimal", "fileobj"),
                 os.path.join("pytrimal", "impl"),
-                os.path.join("vendor", "cpu_features", "include"),
                 "pytrimal",
                 "include",
             ],
             libraries=[
-                "cpu_features",
                 "trimal",
             ],
             depends=[
                 os.path.join("pytrimal", "impl", "template.h"),
             ]
         ),
     ],
```

### Comparing `pytrimal-0.5.5/vendor/trimal/AUTHORS` & `pytrimal-0.6.0/vendor/trimal/AUTHORS`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/CHANGELOG` & `pytrimal-0.6.0/vendor/trimal/CHANGELOG`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/CMakeLists.txt` & `pytrimal-0.6.0/vendor/trimal/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/LICENSE` & `pytrimal-0.6.0/vendor/trimal/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/README.md` & `pytrimal-0.6.0/vendor/trimal/README.md`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.005.AA.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.005.AA.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.006.AA.pir` & `pytrimal-0.6.0/vendor/trimal/dataset/example.006.AA.pir`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.007.AA.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.007.AA.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.007.AA.only_seqs` & `pytrimal-0.6.0/vendor/trimal/dataset/example.007.AA.only_seqs`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.009.AA.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.009.AA.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.010.AA.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.010.AA.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.011.AA.YKL197C.clw` & `pytrimal-0.6.0/vendor/trimal/dataset/example.011.AA.YKL197C.clw`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.011.AA.YKL197C.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.011.AA.YKL197C.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.011.AA.YKL197C.phy` & `pytrimal-0.6.0/vendor/trimal/dataset/example.011.AA.YKL197C.phy`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.012.AA.SuperAlignment.phy` & `pytrimal-0.6.0/vendor/trimal/dataset/example.012.AA.SuperAlignment.phy`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.013.AA.SuperAlignment.phy` & `pytrimal-0.6.0/vendor/trimal/dataset/example.013.AA.SuperAlignment.phy`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.014.AA.EggNOG.COG0591.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.014.AA.EggNOG.COG0591.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.015.AA.bctoNOG.ENOG41099F3.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.015.AA.bctoNOG.ENOG41099F3.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.016.AA.bctoNOG.ENOG41099FB.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.016.AA.bctoNOG.ENOG41099FB.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.017.AA.bctoNOG.ENOG41099FJ.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.017.AA.bctoNOG.ENOG41099FJ.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.018.AA.bctoNOG.ENOG41099FV.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.018.AA.bctoNOG.ENOG41099FV.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.019.AA.bctoNOG.ENOG41099HI.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.019.AA.bctoNOG.ENOG41099HI.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.020.AA.bctoNOG.ENOG41099HN.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.020.AA.bctoNOG.ENOG41099HN.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.021.AA.bctoNOG.ENOG41099I5.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.021.AA.bctoNOG.ENOG41099I5.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.022.AA.bctoNOG.ENOG41099IZ.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.022.AA.bctoNOG.ENOG41099IZ.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.023.AA.bctoNOG.ENOG41099K3.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.023.AA.bctoNOG.ENOG41099K3.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.024.AA.bctoNOG.ENOG41099KM.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.024.AA.bctoNOG.ENOG41099KM.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.025.AA.bctoNOG.ENOG41099KP.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.025.AA.bctoNOG.ENOG41099KP.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.026.AA.bctoNOG.ENOG41099MV.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.026.AA.bctoNOG.ENOG41099MV.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.027.AA.bctoNOG.ENOG41099NY.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.027.AA.bctoNOG.ENOG41099NY.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.028.AA.bctoNOG.ENOG41099PA.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.028.AA.bctoNOG.ENOG41099PA.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.029.AA.bctoNOG.ENOG41099Q3.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.029.AA.bctoNOG.ENOG41099Q3.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.030.AA.bctoNOG.ENOG41099RG.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.030.AA.bctoNOG.ENOG41099RG.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.031.AA.bctoNOG.ENOG41099UK.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.031.AA.bctoNOG.ENOG41099UK.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.032.AA.bctoNOG.ENOG41099UW.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.032.AA.bctoNOG.ENOG41099UW.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.033.AA.bctoNOG.ENOG41099VK.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.033.AA.bctoNOG.ENOG41099VK.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.034.AA.bctoNOG.ENOG41099WA.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.034.AA.bctoNOG.ENOG41099WA.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.035.AA.bctoNOG.ENOG41099WF.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.035.AA.bctoNOG.ENOG41099WF.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.036.AA.bctoNOG.ENOG41099XJ.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.036.AA.bctoNOG.ENOG41099XJ.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.037.AA.bctoNOG.ENOG41099XP.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.037.AA.bctoNOG.ENOG41099XP.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.038.AA.bctoNOG.ENOG41099Y4.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.038.AA.bctoNOG.ENOG41099Y4.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.039.AA.bctoNOG.ENOG41099YD.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.039.AA.bctoNOG.ENOG41099YD.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.040.AA.bctoNOG.ENOG4109A32.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.040.AA.bctoNOG.ENOG4109A32.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.041.AA.bctoNOG.ENOG4109A5T.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.041.AA.bctoNOG.ENOG4109A5T.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.042.AA.bctoNOG.ENOG4109A9M.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.042.AA.bctoNOG.ENOG4109A9M.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.043.AA.bctoNOG.ENOG4109ADN.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.043.AA.bctoNOG.ENOG4109ADN.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.044.AA.bctoNOG.ENOG4109AED.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.044.AA.bctoNOG.ENOG4109AED.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.045.AA.bctoNOG.ENOG4109AGT.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.045.AA.bctoNOG.ENOG4109AGT.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.046.AA.bctoNOG.ENOG4109AGW.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.046.AA.bctoNOG.ENOG4109AGW.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.047.AA.bctoNOG.ENOG4109AIC.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.047.AA.bctoNOG.ENOG4109AIC.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.048.AA.bctoNOG.ENOG4109AJ3.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.048.AA.bctoNOG.ENOG4109AJ3.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.049.AA.bctoNOG.ENOG4109AY5.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.049.AA.bctoNOG.ENOG4109AY5.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.050.AA.bctoNOG.ENOG4109B8Z.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.050.AA.bctoNOG.ENOG4109B8Z.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.051.AA.bctoNOG.ENOG4109BCJ.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.051.AA.bctoNOG.ENOG4109BCJ.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.052.AA.bctoNOG.ENOG4109CTU.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.052.AA.bctoNOG.ENOG4109CTU.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.053.AA.bctoNOG.ENOG4109CVC.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.053.AA.bctoNOG.ENOG4109CVC.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.054.AA.bctoNOG.ENOG4109FIT.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.054.AA.bctoNOG.ENOG4109FIT.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.055.AA.bctoNOG.ENOG4109GY9.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.055.AA.bctoNOG.ENOG4109GY9.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.056.AA.bctoNOG.ENOG4109IPJ.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.056.AA.bctoNOG.ENOG4109IPJ.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.057.AA.bctoNOG.ENOG4109SZ2.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.057.AA.bctoNOG.ENOG4109SZ2.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.058.AA.strNOG.ENOG411BBR6.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.058.AA.strNOG.ENOG411BBR6.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.059.AA.strNOG.ENOG411BBRR.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.059.AA.strNOG.ENOG411BBRR.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.060.AA.strNOG.ENOG411BBWK.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.060.AA.strNOG.ENOG411BBWK.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.061.AA.strNOG.ENOG411BCDZ.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.061.AA.strNOG.ENOG411BCDZ.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.062.AA.strNOG.ENOG411BCX3.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.062.AA.strNOG.ENOG411BCX3.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.063.AA.strNOG.ENOG411BDBU.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.063.AA.strNOG.ENOG411BDBU.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.064.AA.strNOG.ENOG411BDKC.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.064.AA.strNOG.ENOG411BDKC.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.065.AA.strNOG.ENOG411BDSZ.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.065.AA.strNOG.ENOG411BDSZ.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.066.AA.strNOG.ENOG411BDUE.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.066.AA.strNOG.ENOG411BDUE.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.067.AA.strNOG.ENOG411BDX3.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.067.AA.strNOG.ENOG411BDX3.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.068.AA.strNOG.ENOG411BE45.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.068.AA.strNOG.ENOG411BE45.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.069.AA.strNOG.ENOG411BE8B.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.069.AA.strNOG.ENOG411BE8B.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.070.AA.strNOG.ENOG411BEUV.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.070.AA.strNOG.ENOG411BEUV.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.071.AA.strNOG.ENOG411BEZ0.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.071.AA.strNOG.ENOG411BEZ0.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.072.AA.strNOG.ENOG411BF1S.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.072.AA.strNOG.ENOG411BF1S.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.073.AA.strNOG.ENOG411BFCW.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.073.AA.strNOG.ENOG411BFCW.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.074.AA.strNOG.ENOG411BFPF.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.074.AA.strNOG.ENOG411BFPF.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.075.AA.strNOG.ENOG411BFQS.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.075.AA.strNOG.ENOG411BFQS.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.076.AA.strNOG.ENOG411BH75.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.076.AA.strNOG.ENOG411BH75.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.077.AA.strNOG.ENOG411BH79.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.077.AA.strNOG.ENOG411BH79.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.078.AA.strNOG.ENOG411BH99.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.078.AA.strNOG.ENOG411BH99.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.079.AA.strNOG.ENOG411BJDC.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.079.AA.strNOG.ENOG411BJDC.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.080.AA.strNOG.ENOG411BJIF.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.080.AA.strNOG.ENOG411BJIF.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.081.AA.strNOG.ENOG411BK9X.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.081.AA.strNOG.ENOG411BK9X.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.082.AA.strNOG.ENOG411BKC5.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.082.AA.strNOG.ENOG411BKC5.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.083.AA.strNOG.ENOG411BMKC.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.083.AA.strNOG.ENOG411BMKC.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.084.AA.strNOG.ENOG411BNP9.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.084.AA.strNOG.ENOG411BNP9.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.085.AA.strNOG.ENOG411BQTJ.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.085.AA.strNOG.ENOG411BQTJ.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.086.AA.strNOG.ENOG411BR1D.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.086.AA.strNOG.ENOG411BR1D.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.087.AA.strNOG.ENOG411BRCH.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.087.AA.strNOG.ENOG411BRCH.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.088.AA.strNOG.ENOG411BSXF.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.088.AA.strNOG.ENOG411BSXF.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.089.AA.strNOG.ENOG411BV9B.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.089.AA.strNOG.ENOG411BV9B.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.090.AA.strNOG.ENOG411BVKR.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.090.AA.strNOG.ENOG411BVKR.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.091.AA.strNOG.ENOG411BWBU.codon.fa` & `pytrimal-0.6.0/vendor/trimal/dataset/example.091.AA.strNOG.ENOG411BWBU.codon.fa`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.091.AA.strNOG.ENOG411BWBU.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.091.AA.strNOG.ENOG411BWBU.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.092.DNA.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.092.DNA.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.093.DNA.fasta` & `pytrimal-0.6.0/vendor/trimal/dataset/example.093.DNA.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/example.094.DNADeg.sequential_phy` & `pytrimal-0.6.0/vendor/trimal/dataset/example.094.DNADeg.sequential_phy`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/dataset/matrix.BLOSUM62` & `pytrimal-0.6.0/vendor/trimal/dataset/matrix.BLOSUM62`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/Alignment/Alignment.h` & `pytrimal-0.6.0/vendor/trimal/include/Alignment/Alignment.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/Alignment/sequencesMatrix.h` & `pytrimal-0.6.0/vendor/trimal/include/Alignment/sequencesMatrix.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/Cleaner.h` & `pytrimal-0.6.0/vendor/trimal/include/Cleaner.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/BaseFormatHandler.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/BaseFormatHandler.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/FormatManager.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/FormatManager.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/clustal_state.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/clustal_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/fasta_m10_state.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/fasta_m10_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/fasta_state.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/fasta_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/formats_header.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/formats_header.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/htmlreport_state.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/htmlreport_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/mega_interleaved_state.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/mega_interleaved_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/mega_sequential_state.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/mega_sequential_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/nexus_m10_state.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/nexus_m10_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/nexus_state.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/nexus_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/phylip32_m10_state.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip32_m10_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/phylip32_state.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip32_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/phylip40_m10_state.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip40_m10_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/phylip40_state.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip40_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/phylip_paml_m10_state.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip_paml_m10_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/phylip_paml_state.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip_paml_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/FormatHandling/pir_state.h` & `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/pir_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/InternalBenchmarker.h` & `pytrimal-0.6.0/vendor/trimal/include/InternalBenchmarker.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/RawText/examples.txt` & `pytrimal-0.6.0/vendor/trimal/include/RawText/examples.txt`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/RawText/legacyMenu.txt` & `pytrimal-0.6.0/vendor/trimal/include/RawText/legacyMenu.txt`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/RawText/menu.txt` & `pytrimal-0.6.0/vendor/trimal/include/RawText/menu.txt`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/Statistics/Consistency.h` & `pytrimal-0.6.0/vendor/trimal/include/Statistics/Consistency.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/Statistics/Gaps.h` & `pytrimal-0.6.0/vendor/trimal/include/Statistics/Gaps.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/Statistics/Manager.h` & `pytrimal-0.6.0/vendor/trimal/include/Statistics/Manager.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/Statistics/Mold.h` & `pytrimal-0.6.0/vendor/trimal/include/Statistics/Mold.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/Statistics/Similarity.h` & `pytrimal-0.6.0/vendor/trimal/include/Statistics/Similarity.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/Statistics/similarityMatrix.h` & `pytrimal-0.6.0/vendor/trimal/include/Statistics/similarityMatrix.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/VCFHandler.h` & `pytrimal-0.6.0/vendor/trimal/include/VCFHandler.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/defines.h` & `pytrimal-0.6.0/vendor/trimal/include/defines.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/reportsystem.h` & `pytrimal-0.6.0/vendor/trimal/include/reportsystem.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/trimalManager.h` & `pytrimal-0.6.0/vendor/trimal/include/trimalManager.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/utils.h` & `pytrimal-0.6.0/vendor/trimal/include/utils.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/include/values.h` & `pytrimal-0.6.0/vendor/trimal/include/values.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/Alignment/Alignment.cpp` & `pytrimal-0.6.0/vendor/trimal/source/Alignment/Alignment.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/Alignment/sequencesMatrix.cpp` & `pytrimal-0.6.0/vendor/trimal/source/Alignment/sequencesMatrix.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/Cleaner.cpp` & `pytrimal-0.6.0/vendor/trimal/source/Cleaner.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/BaseFormatHandler.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/BaseFormatHandler.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/clustal_state.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/clustal_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/fasta_m10_state.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/fasta_m10_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/fasta_state.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/fasta_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/htmlreport_state.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/htmlreport_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/mega_interleaved_state.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/mega_interleaved_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/mega_sequential_state.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/mega_sequential_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/nexus_m10_state.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/nexus_m10_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/nexus_state.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/nexus_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/phylip32_m10_state.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip32_m10_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/phylip32_state.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip32_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/phylip40_m10_state.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip40_m10_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/phylip40_state.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip40_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/phylip_paml_m10_state.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip_paml_m10_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/phylip_paml_state.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip_paml_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/pir_state.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/pir_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/FormatHandling/readAlMain.cpp` & `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/readAlMain.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/InternalBenchmarker.cpp` & `pytrimal-0.6.0/vendor/trimal/source/InternalBenchmarker.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/Statistics/Consistency.cpp` & `pytrimal-0.6.0/vendor/trimal/source/Statistics/Consistency.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/Statistics/Gaps.cpp` & `pytrimal-0.6.0/vendor/trimal/source/Statistics/Gaps.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/Statistics/Manager.cpp` & `pytrimal-0.6.0/vendor/trimal/source/Statistics/Manager.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/Statistics/Mold.cpp` & `pytrimal-0.6.0/vendor/trimal/source/Statistics/Mold.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/Statistics/Similarity.cpp` & `pytrimal-0.6.0/vendor/trimal/source/Statistics/Similarity.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/Statistics/similarityMatrix.cpp` & `pytrimal-0.6.0/vendor/trimal/source/Statistics/similarityMatrix.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/VCFHandler.cpp` & `pytrimal-0.6.0/vendor/trimal/source/VCFHandler.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/alignment.cpp` & `pytrimal-0.6.0/vendor/trimal/source/alignment.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/compareFiles.cpp` & `pytrimal-0.6.0/vendor/trimal/source/compareFiles.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/main.cpp` & `pytrimal-0.6.0/vendor/trimal/source/main.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/reportMessages/errorMessages.cpp` & `pytrimal-0.6.0/vendor/trimal/source/reportMessages/errorMessages.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/reportMessages/infoMessages.cpp` & `pytrimal-0.6.0/vendor/trimal/source/reportMessages/infoMessages.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/reportMessages/warningMessages.cpp` & `pytrimal-0.6.0/vendor/trimal/source/reportMessages/warningMessages.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/reportsystem.cpp` & `pytrimal-0.6.0/vendor/trimal/source/reportsystem.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/rwAlignment.cpp` & `pytrimal-0.6.0/vendor/trimal/source/rwAlignment.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/trimAlMain.cpp` & `pytrimal-0.6.0/vendor/trimal/source/trimAlMain.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/trimalManager.cpp` & `pytrimal-0.6.0/vendor/trimal/source/trimalManager.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/typeHelper.cpp` & `pytrimal-0.6.0/vendor/trimal/source/typeHelper.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.5.5/vendor/trimal/source/utils.cpp` & `pytrimal-0.6.0/vendor/trimal/source/utils.cpp`

 * *Files identical despite different names*

