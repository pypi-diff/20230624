# Comparing `tmp/pyjson5-1.6.2.tar.gz` & `tmp/pyjson5-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjson5-1.6.2.tar", last modified: Wed Sep 14 22:40:35 2022, max compression
+gzip compressed data, was "pyjson5-1.6.3.tar", last modified: Fri Jun 23 22:35:50 2023, max compression
```

## Comparing `pyjson5-1.6.2.tar` & `pyjson5-1.6.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2022-09-14 22:40:35.357656 pyjson5-1.6.2/
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)    11358 2021-11-17 20:47:55.000000 pyjson5-1.6.2/LICENSE
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      293 2022-06-07 15:42:23.000000 pyjson5-1.6.2/MANIFEST.in
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1626 2022-09-14 22:35:46.000000 pyjson5-1.6.2/Makefile
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2477 2022-09-14 22:40:35.357656 pyjson5-1.6.2/PKG-INFO
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1205 2021-11-17 20:47:55.000000 pyjson5-1.6.2/README.rst
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2022-09-14 22:40:35.353656 pyjson5-1.6.2/docs/
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2195 2022-09-14 22:39:06.000000 pyjson5-1.6.2/docs/changelog.md
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1765 2021-11-17 21:09:25.000000 pyjson5-1.6.2/docs/conf.py
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1707 2021-11-17 20:47:55.000000 pyjson5-1.6.2/docs/decoder.rst
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1581 2021-11-17 20:47:55.000000 pyjson5-1.6.2/docs/encoder.rst
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      400 2021-11-17 20:47:55.000000 pyjson5-1.6.2/docs/exceptions.rst
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1590 2021-11-17 21:27:24.000000 pyjson5-1.6.2/docs/index.rst
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     7725 2021-11-17 20:47:55.000000 pyjson5-1.6.2/docs/performance.rst
--rwxr-xr-x   0 kijewski  (1000) kijewski  (1000)     2076 2021-11-17 20:47:55.000000 pyjson5-1.6.2/make_decoder_recursive_select.py
--rwxr-xr-x   0 kijewski  (1000) kijewski  (1000)     1648 2021-11-17 20:47:55.000000 pyjson5-1.6.2/make_escape_dct.py
--rwxr-xr-x   0 kijewski  (1000) kijewski  (1000)     4581 2021-11-17 20:47:55.000000 pyjson5-1.6.2/make_unicode_categories.py
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)  2203292 2022-09-14 22:36:42.000000 pyjson5-1.6.2/pyjson5.cpp
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1402 2021-11-17 20:47:55.000000 pyjson5-1.6.2/pyjson5.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      115 2022-01-18 17:59:45.000000 pyjson5-1.6.2/pyproject.toml
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1379 2022-09-14 22:40:35.357656 pyjson5-1.6.2/setup.cfg
--rwxr-xr-x   0 kijewski  (1000) kijewski  (1000)      450 2022-01-18 17:59:45.000000 pyjson5-1.6.2/setup.py
--rwxr-xr-x   0 kijewski  (1000) kijewski  (1000)     1039 2021-11-17 20:47:55.000000 pyjson5-1.6.2/sha512sum.py
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2022-09-14 22:40:35.357656 pyjson5-1.6.2/src/
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      717 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/DESCRIPTION.inc
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)        8 2022-09-14 22:39:47.000000 pyjson5-1.6.2/src/VERSION.inc
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      642 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_constants.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)    24579 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_decoder.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1851 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_decoder_recursive_select.hpp
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)    13753 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_encoder.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     5514 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_encoder_options.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)    15851 2022-09-14 22:36:39.000000 pyjson5-1.6.2/src/_escape_dct.hpp
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      324 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_exceptions.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2153 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_exceptions_decoder.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      598 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_exceptions_encoder.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)    17237 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_exports.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     6734 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_imports.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2032 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_legacy.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2384 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_raise_decoder.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      303 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_raise_encoder.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1084 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_reader_callback.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1891 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_reader_ucs.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1016 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_readers.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2434 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_stack_heap_string.hpp
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1345 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_unicode.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)   620667 2022-09-14 22:36:40.000000 pyjson5-1.6.2/src/_unicode_cat_of.hpp
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1073 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_writer_callback.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      385 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_writer_noop.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1630 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_writer_reallocatable.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      290 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/_writers.pyx
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)    58461 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/dragonbox.cc
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     5183 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/native.hpp
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2022-09-14 22:40:35.357656 pyjson5-1.6.2/src/pyjson5/
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)       99 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/pyjson5/__init__.py
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     8430 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/pyjson5/__init__.pyi
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)        0 2021-11-17 20:47:55.000000 pyjson5-1.6.2/src/pyjson5/py.typed
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2022-09-14 22:40:35.357656 pyjson5-1.6.2/src/pyjson5.egg-info/
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2477 2022-09-14 22:40:35.000000 pyjson5-1.6.2/src/pyjson5.egg-info/PKG-INFO
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1209 2022-09-14 22:40:35.000000 pyjson5-1.6.2/src/pyjson5.egg-info/SOURCES.txt
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)        1 2022-09-14 22:40:35.000000 pyjson5-1.6.2/src/pyjson5.egg-info/dependency_links.txt
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)        1 2021-11-17 20:51:40.000000 pyjson5-1.6.2/src/pyjson5.egg-info/not-zip-safe
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)        8 2022-09-14 22:40:35.000000 pyjson5-1.6.2/src/pyjson5.egg-info/top_level.txt
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2022-09-14 22:40:35.351656 pyjson5-1.6.2/third-party/
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2022-09-14 22:40:35.351656 pyjson5-1.6.2/third-party/fast_double_parser/
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2022-09-14 22:40:35.357656 pyjson5-1.6.2/third-party/fast_double_parser/include/
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)    50269 2022-06-02 23:27:37.000000 pyjson5-1.6.2/third-party/fast_double_parser/include/fast_double_parser.h
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-06-23 22:35:50.088080 pyjson5-1.6.3/
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)    11358 2021-11-17 20:47:55.000000 pyjson5-1.6.3/LICENSE
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      293 2022-06-07 15:42:23.000000 pyjson5-1.6.3/MANIFEST.in
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1567 2023-06-23 22:12:07.000000 pyjson5-1.6.3/Makefile
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2907 2023-06-23 22:35:50.088080 pyjson5-1.6.3/PKG-INFO
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1205 2021-11-17 20:47:55.000000 pyjson5-1.6.3/README.rst
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-06-23 22:35:50.084079 pyjson5-1.6.3/docs/
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2288 2023-06-23 22:12:07.000000 pyjson5-1.6.3/docs/changelog.md
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1238 2023-06-23 22:12:07.000000 pyjson5-1.6.3/docs/conf.py
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1731 2023-06-23 22:12:07.000000 pyjson5-1.6.3/docs/decoder.rst
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1589 2023-06-23 22:12:07.000000 pyjson5-1.6.3/docs/encoder.rst
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      404 2023-06-23 22:12:07.000000 pyjson5-1.6.3/docs/exceptions.rst
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1590 2021-11-17 21:27:24.000000 pyjson5-1.6.3/docs/index.rst
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     7725 2021-11-17 20:47:55.000000 pyjson5-1.6.3/docs/performance.rst
+-rwxr-xr-x   0 kijewski  (1000) kijewski  (1000)     2104 2023-06-23 22:12:07.000000 pyjson5-1.6.3/make_decoder_recursive_select.py
+-rwxr-xr-x   0 kijewski  (1000) kijewski  (1000)     1714 2023-06-23 22:12:07.000000 pyjson5-1.6.3/make_escape_dct.py
+-rwxr-xr-x   0 kijewski  (1000) kijewski  (1000)     4711 2023-06-23 22:12:07.000000 pyjson5-1.6.3/make_unicode_categories.py
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)  2206865 2023-06-23 21:32:45.000000 pyjson5-1.6.3/pyjson5.cpp
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1392 2023-06-23 22:12:07.000000 pyjson5-1.6.3/pyjson5.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      102 2023-06-23 22:12:07.000000 pyjson5-1.6.3/pyproject.toml
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1741 2023-06-23 22:35:50.088080 pyjson5-1.6.3/setup.cfg
+-rwxr-xr-x   0 kijewski  (1000) kijewski  (1000)      512 2023-06-23 22:12:07.000000 pyjson5-1.6.3/setup.py
+-rwxr-xr-x   0 kijewski  (1000) kijewski  (1000)     1044 2023-06-23 22:12:07.000000 pyjson5-1.6.3/sha512sum.py
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-06-23 22:35:50.086079 pyjson5-1.6.3/src/
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      717 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/DESCRIPTION.inc
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)        8 2023-06-23 22:12:07.000000 pyjson5-1.6.3/src/VERSION.inc
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      642 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_constants.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)    24579 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_decoder.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1851 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_decoder_recursive_select.hpp
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)    13753 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_encoder.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     5514 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_encoder_options.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)    15851 2023-06-23 21:23:34.000000 pyjson5-1.6.3/src/_escape_dct.hpp
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      324 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_exceptions.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2153 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_exceptions_decoder.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      598 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_exceptions_encoder.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)    17225 2023-06-23 22:12:07.000000 pyjson5-1.6.3/src/_exports.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     6734 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_imports.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2032 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_legacy.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2384 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_raise_decoder.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      303 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_raise_encoder.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1084 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_reader_callback.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1891 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_reader_ucs.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1016 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_readers.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2434 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_stack_heap_string.hpp
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1345 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_unicode.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)   620667 2023-06-23 21:23:34.000000 pyjson5-1.6.3/src/_unicode_cat_of.hpp
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1073 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_writer_callback.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      385 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_writer_noop.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1630 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_writer_reallocatable.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      290 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/_writers.pyx
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)    58461 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/dragonbox.cc
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     5183 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/native.hpp
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-06-23 22:35:50.086079 pyjson5-1.6.3/src/pyjson5/
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)       99 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/pyjson5/__init__.py
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     8303 2023-06-23 22:12:07.000000 pyjson5-1.6.3/src/pyjson5/__init__.pyi
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)        0 2021-11-17 20:47:55.000000 pyjson5-1.6.3/src/pyjson5/py.typed
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-06-23 22:35:50.088080 pyjson5-1.6.3/src/pyjson5.egg-info/
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2907 2023-06-23 22:35:50.000000 pyjson5-1.6.3/src/pyjson5.egg-info/PKG-INFO
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1209 2023-06-23 22:35:50.000000 pyjson5-1.6.3/src/pyjson5.egg-info/SOURCES.txt
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)        1 2023-06-23 22:35:50.000000 pyjson5-1.6.3/src/pyjson5.egg-info/dependency_links.txt
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)        1 2021-11-17 20:51:40.000000 pyjson5-1.6.3/src/pyjson5.egg-info/not-zip-safe
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)        8 2023-06-23 22:35:50.000000 pyjson5-1.6.3/src/pyjson5.egg-info/top_level.txt
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-06-23 22:35:50.080079 pyjson5-1.6.3/third-party/
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-06-23 22:35:50.080079 pyjson5-1.6.3/third-party/fast_double_parser/
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-06-23 22:35:50.088080 pyjson5-1.6.3/third-party/fast_double_parser/include/
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)    50269 2022-06-02 23:27:37.000000 pyjson5-1.6.3/third-party/fast_double_parser/include/fast_double_parser.h
```

### Comparing `pyjson5-1.6.2/LICENSE` & `pyjson5-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/Makefile` & `pyjson5-1.6.3/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-all: sdist bdist_wheel docs
+all: sdist wheel docs
 
 .DELETE_ON_ERROR:
 
-.PHONY: all sdist bdist_wheel clean docs prepare test install
+.PHONY: all sdist wheel clean docs prepare test install
 
 export PYTHONUTF8 := 1
 export PYTHONIOENCODING := UTF-8
 
 INCLUDES := \
     src/VERSION.inc src/DESCRIPTION.inc \
     src/_decoder_recursive_select.hpp src/_unicode_cat_of.hpp \
@@ -30,30 +30,30 @@
 
 pyjson5.cpp: pyjson5.pyx $(wildcard src/*.pyx) $(wildcard src/*.hpp)
 	python -m cython -f -o $@ $<
 
 prepare: pyjson5.cpp ${FILES}
 
 sdist: prepare
-	rm -f -- dist/pyjson5-*.tar.gz
-	python setup.py sdist
+	-rm -- dist/pyjson5-*.tar.gz
+	python -m build --sdist
 
-bdist_wheel: pyjson5.cpp ${FILES} | sdist
-	rm -f -- dist/pyjson5-*.whl
-	python setup.py bdist_wheel
+wheel: prepare
+	-rm -- dist/pyjson5-*.whl
+	python -m build --wheel
 
-install: bdist_wheel
+install: wheel
 	pip install --force dist/pyjson5-*.whl
 
 docs: install $(wildcard docs/* docs/*/*)
 	python -m sphinx -M html docs/ dist/
 
 clean:
 	[ ! -d build/ ] || rm -r -- build/
 	[ ! -d dist/ ] || rm -r -- dist/
 	[ ! -d pyjson5.egg-info/ ] || rm -r -- pyjson5.egg-info/
-	rm -f -- pyjson5.*.so python5.cpp
+	-rm -- pyjson5.*.so python5.cpp
 
-test: bdist_wheel
+test: wheel
 	pip install --force dist/pyjson5-*.whl
 	python run-minefield-test.py
 	python run-tests.py
```

### Comparing `pyjson5-1.6.2/README.rst` & `pyjson5-1.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/docs/changelog.md` & `pyjson5-1.6.3/docs/changelog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+**1.6.3**
+
+* Fix typing for `dump()` ([#61](https://github.com/Kijewski/pyjson5/issues/61))
+
 **1.6.2**
 
 * Update to Unicode 15.0.0
 
 **1.6.1**
 
 * Fix [PEP 517](https://www.python.org/dev/peps/pep-0517/)-like installation using [build](https://github.com/pypa/build) (by [Tomasz Kłoczko](https://github.com/kloczek))
```

### Comparing `pyjson5-1.6.2/docs/conf.py` & `pyjson5-1.6.3/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,66 +12,42 @@
     'sphinx.ext.intersphinx',
     'sphinx.ext.inheritance_diagram',
     'sphinx_autodoc_typehints',
     'sphinx.ext.autosectionlabel',
     'myst_parser',
 ]
 
+language = "en"
+
 templates_path = ['_templates']
 source_suffix = '.rst'
 master_doc = 'index'
 
-project = u'PyJSON5'
-copyright = u'2018-2021, René Kijewski'
-author = u'René Kijewski'
+project = 'PyJSON5'
+copyright = '2018-2023, René Kijewski'
+author = 'René Kijewski'
 
 with open('../src/VERSION.inc', 'rt') as f:
     version = eval(f.read().strip())
     release = version
 
 language = None
 exclude_patterns = []
 pygments_style = 'sphinx'
 todo_include_todos = False
 
-html_theme = 'sphinx_rtd_theme'
-html_theme_options = {
-    'navigation_depth': -1,
-}
-html_sidebars = {
-    '**': [
-        'localtoc.html',
-        'searchbox.html',
-    ]
-}
+html_theme = 'furo'
 htmlhelp_basename = 'PyJSON5doc'
 
-latex_elements = {}
-latex_documents = [
-    (master_doc, 'PyJSON5.tex', u'PyJSON5 Documentation',
-     u'René Kijewski', 'manual'),
-]
-
-man_pages = [
-    (master_doc, 'pyjson5', u'PyJSON5 Documentation',
-     [author], 1)
-]
-
-texinfo_documents = [
-    (master_doc, 'PyJSON5', u'PyJSON5 Documentation',
-     author, 'PyJSON5', 'One line description of project.',
-     'Miscellaneous'),
-]
-
 display_toc = True
 autodoc_default_flags = ['members']
 autosummary_generate = True
 
 intersphinx_mapping = {
-    'python': ('https://docs.python.org/3.10', None),
+    'python': ('https://docs.python.org/3.11', None),
 }
 
 inheritance_graph_attrs = {
     'size': '"6.0, 8.0"',
     'fontsize': 32,
     'bgcolor': 'transparent',
 }
```

### Comparing `pyjson5-1.6.2/docs/decoder.rst` & `pyjson5-1.6.3/docs/decoder.rst`

 * *Files 12% similar despite different names*

```diff
@@ -55,30 +55,30 @@
     pyjson5.Json5DecoderException
     pyjson5.Json5NestingTooDeep
     pyjson5.Json5EOF
     pyjson5.Json5IllegalCharacter
     pyjson5.Json5ExtraData
     pyjson5.Json5IllegalType
 
-.. autoclass:: pyjson5.Json5DecoderException
+.. autoexception:: pyjson5.Json5DecoderException
     :members:
     :inherited-members:
 
-.. autoclass:: pyjson5.Json5NestingTooDeep
+.. autoexception:: pyjson5.Json5NestingTooDeep
     :members:
     :inherited-members:
 
-.. autoclass:: pyjson5.Json5EOF
+.. autoexception:: pyjson5.Json5EOF
     :members:
     :inherited-members:
 
-.. autoclass:: pyjson5.Json5IllegalCharacter
+.. autoexception:: pyjson5.Json5IllegalCharacter
     :members:
     :inherited-members:
 
-.. autoclass:: pyjson5.Json5ExtraData
+.. autoexception:: pyjson5.Json5ExtraData
     :members:
     :inherited-members:
 
-.. autoclass:: pyjson5.Json5IllegalType
+.. autoexception:: pyjson5.Json5IllegalType
     :members:
     :inherited-members:
```

### Comparing `pyjson5-1.6.2/docs/encoder.rst` & `pyjson5-1.6.3/docs/encoder.rst`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,14 @@
 ------------------
 
 .. inheritance-diagram::
     pyjson5.Json5Exception
     pyjson5.Json5EncoderException
     pyjson5.Json5UnstringifiableType
 
-.. autoclass:: pyjson5.Json5EncoderException
+.. autoexception:: pyjson5.Json5EncoderException
     :members:
     :inherited-members:
 
-.. autoclass:: pyjson5.Json5UnstringifiableType
+.. autoexception:: pyjson5.Json5UnstringifiableType
     :members:
     :inherited-members:
```

### Comparing `pyjson5-1.6.2/docs/index.rst` & `pyjson5-1.6.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/docs/performance.rst` & `pyjson5-1.6.3/docs/performance.rst`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/make_escape_dct.py` & `pyjson5-1.6.3/make_escape_dct.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,51 +3,60 @@
 from argparse import ArgumentParser
 from logging import basicConfig, DEBUG
 from pathlib import Path
 
 
 def generate(f):
     unescaped = 0
-    print('const EscapeDct::Items EscapeDct::items = {', file=f)
+    print("const EscapeDct::Items EscapeDct::items = {", file=f)
     for c in range(0x100):
-        if c == ord('\\'):
-            s = '\\\\'
-        elif c == ord('\b'):
-            s = '\\b'
-        elif c == ord('\f'):
-            s = '\\f'
-        elif c == ord('\n'):
-            s = '\\n'
-        elif c == ord('\r'):
-            s = '\\r'
-        elif c == ord('\t'):
-            s = '\\t'
+        if c == ord("\\"):
+            s = "\\\\"
+        elif c == ord("\b"):
+            s = "\\b"
+        elif c == ord("\f"):
+            s = "\\f"
+        elif c == ord("\n"):
+            s = "\\n"
+        elif c == ord("\r"):
+            s = "\\r"
+        elif c == ord("\t"):
+            s = "\\t"
         elif c == ord('"'):
             s = '\\"'
-        elif (c < 0x20) or (c >= 0x7f) or (chr(c) in "'&<>\\"):
-            s = f'\\u{c:04x}'
+        elif (c < 0x20) or (c >= 0x7F) or (chr(c) in "'&<>\\"):
+            s = f"\\u{c:04x}"
         else:
-            s = f'{c:c}'
+            s = f"{c:c}"
             if c < 128:
                 unescaped |= 1 << c
 
-        t = [str(len(s))] + [
-            f"'{c}'" if c != '\\' else f"'\\\\'"
-            for c in s
-        ] + ['0'] * 6
-        l = ', '.join(t[:8])
-        print(f'   {{ {l:35s} }},  /* 0x{c:02x} {chr(c)!r} */', file=f)
-    print('};', file=f)
+        t = (
+            [str(len(s))]
+            + [f"'{c}'" if c != "\\" else f"'\\\\'" for c in s]
+            + ["0"] * 6
+        )
+        l = ", ".join(t[:8])
+        print(f"   {{ {l:35s} }},  /* 0x{c:02x} {chr(c)!r} */", file=f)
+    print("};", file=f)
 
     escaped = unescaped ^ ((1 << 128) - 1)
-    print(f'const std::uint64_t EscapeDct::is_escaped_lo = UINT64_C(0x{(escaped & ((1 << 64) - 1)):016x});', file=f)
-    print(f'const std::uint64_t EscapeDct::is_escaped_hi = UINT64_C(0x{(escaped >> 64):016x});', file=f)
+    print(
+        f"const std::uint64_t EscapeDct::is_escaped_lo = UINT64_C(0x{(escaped & ((1 << 64) - 1)):016x});",
+        file=f,
+    )
+    print(
+        f"const std::uint64_t EscapeDct::is_escaped_hi = UINT64_C(0x{(escaped >> 64):016x});",
+        file=f,
+    )
+
+
+argparser = ArgumentParser(description="Generate src/_escape_dct.hpp")
+argparser.add_argument(
+    "input", nargs="?", type=Path, default=Path("src/_escape_dct.hpp")
+)
 
-
-argparser = ArgumentParser(description='Generate src/_escape_dct.hpp')
-argparser.add_argument('input', nargs='?', type=Path, default=Path('src/_escape_dct.hpp'))
-
-if __name__ == '__main__':
+if __name__ == "__main__":
     basicConfig(level=DEBUG)
     args = argparser.parse_args()
-    with open(str(args.input.resolve()), 'wt') as out:
+    with open(str(args.input.resolve()), "wt") as out:
         generate(out)
```

### Comparing `pyjson5-1.6.2/make_unicode_categories.py` & `pyjson5-1.6.3/make_unicode_categories.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,111 +12,125 @@
 def main(input_file, output_file):
     Nothing = 0
     WhiteSpace = 1
     IdentifierStart = 2
     IdentifierPart = 3
 
     cat_indices = {
-        'zs': WhiteSpace,
-
-        'lc': IdentifierStart,
-        'll': IdentifierStart,
-        'lm': IdentifierStart,
-        'lo': IdentifierStart,
-        'lt': IdentifierStart,
-        'lu': IdentifierStart,
-        'nl': IdentifierStart,
-
-        'mc': IdentifierPart,
-        'mn': IdentifierPart,
-        'pc': IdentifierPart,
-        'nd': IdentifierPart,
+        "zs": WhiteSpace,
+        "lc": IdentifierStart,
+        "ll": IdentifierStart,
+        "lm": IdentifierStart,
+        "lo": IdentifierStart,
+        "lt": IdentifierStart,
+        "lu": IdentifierStart,
+        "nl": IdentifierStart,
+        "mc": IdentifierPart,
+        "mn": IdentifierPart,
+        "pc": IdentifierPart,
+        "nd": IdentifierPart,
     }
 
     planes = defaultdict(lambda: [0] * 0x10000)
 
     for input_line in input_file:
-        m = match(r'^([0-9A-F]+)(?:\.\.([0-9A-F]+))?\s+;\s+([A-Z][a-z])', input_line)
+        m = match(r"^([0-9A-F]+)(?:\.\.([0-9A-F]+))?\s+;\s+([A-Z][a-z])", input_line)
         if not m:
             continue
         start, end, cat = m.groups()
 
         idx = cat_indices.get(cat.lower())
         if idx:
             end = int(end or start, 16)
             start = int(start, 16)
             for i in range(start, end + 1):
                 planes[i // 0x10000][i % 0x10000] = idx
 
     # per: https://spec.json5.org/#white-space
-    for i in (0x9, 0xa, 0xb, 0xc, 0xd, 0x20, 0xa0, 0x2028, 0x2028, 0x2029, 0xfeff):
+    for i in (0x9, 0xA, 0xB, 0xC, 0xD, 0x20, 0xA0, 0x2028, 0x2028, 0x2029, 0xFEFF):
         planes[0][i] = WhiteSpace
 
     # per: https://www.ecma-international.org/ecma-262/5.1/#sec-7.6
-    for i in (ord('$'), ord('_'), ord('\\')):
+    for i in (ord("$"), ord("_"), ord("\\")):
         planes[0][i] = IdentifierStart
 
     # per: https://www.ecma-international.org/ecma-262/5.1/#sec-7.6
     for i in (0x200C, 0x200D):
         planes[0][i] = IdentifierPart
 
-    print('#ifndef JSON5EncoderCpp_unicode_cat_of', file=output_file)
-    print('#define JSON5EncoderCpp_unicode_cat_of', file=output_file)
+    print("#ifndef JSON5EncoderCpp_unicode_cat_of", file=output_file)
+    print("#define JSON5EncoderCpp_unicode_cat_of", file=output_file)
     print(file=output_file)
-    print('// GENERATED FILE', file=output_file)
-    print('// All changes will be lost.', file=output_file)
+    print("// GENERATED FILE", file=output_file)
+    print("// All changes will be lost.", file=output_file)
     print(file=output_file)
-    print('#include <cstdint>', file=output_file)
+    print("#include <cstdint>", file=output_file)
     print(file=output_file)
-    print('namespace JSON5EncoderCpp {', file=output_file)
-    print('inline namespace {', file=output_file)
+    print("namespace JSON5EncoderCpp {", file=output_file)
+    print("inline namespace {", file=output_file)
     print(file=output_file)
-    print('static unsigned unicode_cat_of(std::uint32_t codepoint) {', file=output_file)
+    print("static unsigned unicode_cat_of(std::uint32_t codepoint) {", file=output_file)
 
-    print('    static std::uint8_t plane_X[0x10000 / 4] = {0};', file=output_file)
+    print("    static std::uint8_t plane_X[0x10000 / 4] = {0};", file=output_file)
     print(file=output_file)
 
     for plane_idx, plane_data in planes.items():
-        print('    static std::uint8_t plane_' + str(plane_idx) + '[0x10000 / 4] = {', file=output_file)
-        for chunk in chunked(plane_data, 4*16):
-            print('        ', end='', file=output_file)
+        print(
+            "    static std::uint8_t plane_" + str(plane_idx) + "[0x10000 / 4] = {",
+            file=output_file,
+        )
+        for chunk in chunked(plane_data, 4 * 16):
+            print("        ", end="", file=output_file)
             for value in chunked(chunk, 4):
                 value = reduce(lambda a, i: ((a << 2) | i), reversed(value), 0)
-                print('0x{:02x}u'.format(value), end=', ', file=output_file)
+                print("0x{:02x}u".format(value), end=", ", file=output_file)
             print(file=output_file)
-        print('    };', file=output_file)
+        print("    };", file=output_file)
         print(file=output_file)
 
-    print('    static std::uint8_t *planes[17] = {', end='', file=output_file)
+    print("    static std::uint8_t *planes[17] = {", end="", file=output_file)
     for plane_idx in range(0, 17):
         if plane_idx % 8 == 0:
-            print('\n        ', end='', file=output_file)
+            print("\n        ", end="", file=output_file)
         if plane_idx in planes:
-            print('plane_' + str(plane_idx) + ', ', end='', file=output_file)
+            print("plane_" + str(plane_idx) + ", ", end="", file=output_file)
         else:
-            print('plane_X, ', end='', file=output_file)
-    print(file=output_file)
-    print('    };', file=output_file)
+            print("plane_X, ", end="", file=output_file)
     print(file=output_file)
-
-    print('    std::uint16_t plane_idx = std::uint16_t(codepoint / 0x10000);', file=output_file)
-    print('    if (JSON5EncoderCpp_expect(plane_idx > 16, false)) return 1;', file=output_file)
-    print('    std::uint16_t datum_idx = std::uint16_t(codepoint & 0xffff);', file=output_file)
-    print('    const std::uint8_t *plane = planes[plane_idx];', file=output_file)
-    print('    return (plane[datum_idx / 4] >> (2 * (datum_idx % 4))) % 4;', file=output_file)
-    print('}', file=output_file)
+    print("    };", file=output_file)
     print(file=output_file)
-    print('}', file=output_file)
-    print('}', file=output_file)
-    print(file=output_file)
-    print('#endif', file=output_file)
-
 
-argparser = ArgumentParser(description='Generate Unicode Category Matcher(s)')
-argparser.add_argument('input', nargs='?', type=Path, default=Path('/dev/stdin'))
-argparser.add_argument('output', nargs='?', type=Path, default=Path('/dev/stdout'))
+    print(
+        "    std::uint16_t plane_idx = std::uint16_t(codepoint / 0x10000);",
+        file=output_file,
+    )
+    print(
+        "    if (JSON5EncoderCpp_expect(plane_idx > 16, false)) return 1;",
+        file=output_file,
+    )
+    print(
+        "    std::uint16_t datum_idx = std::uint16_t(codepoint & 0xffff);",
+        file=output_file,
+    )
+    print("    const std::uint8_t *plane = planes[plane_idx];", file=output_file)
+    print(
+        "    return (plane[datum_idx / 4] >> (2 * (datum_idx % 4))) % 4;",
+        file=output_file,
+    )
+    print("}", file=output_file)
+    print(file=output_file)
+    print("}", file=output_file)
+    print("}", file=output_file)
+    print(file=output_file)
+    print("#endif", file=output_file)
+
+
+argparser = ArgumentParser(description="Generate Unicode Category Matcher(s)")
+argparser.add_argument("input", nargs="?", type=Path, default=Path("/dev/stdin"))
+argparser.add_argument("output", nargs="?", type=Path, default=Path("/dev/stdout"))
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     args = argparser.parse_args()
-    with open(str(args.input.resolve()), 'rt') as input_file, \
-         open(str(args.output.resolve()), 'wt') as output_file:
+    with open(str(args.input.resolve()), "rt") as input_file, open(
+        str(args.output.resolve()), "wt"
+    ) as output_file:
         raise SystemExit(main(input_file, output_file))
```

### Comparing `pyjson5-1.6.2/pyjson5.cpp` & `pyjson5-1.6.3/pyjson5.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.30 */
+/* Generated by Cython 0.29.35 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_30"
-#define CYTHON_HEX_VERSION 0x001D1EF0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,14 +45,15 @@
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
@@ -73,29 +74,34 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
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
@@ -128,18 +134,64 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
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
@@ -151,15 +203,15 @@
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
@@ -190,15 +242,15 @@
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
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -500,35 +552,35 @@
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
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
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
@@ -929,17 +981,17 @@
   "src/_decoder.pyx",
   "src/_writer_reallocatable.pyx",
   "src/_writer_callback.pyx",
   "src/_encoder.pyx",
   "src/_exports.pyx",
   "src/_legacy.pyx",
   "pyjson5.pyx",
-  "env/lib/python3.10/site-packages/Cython/Includes/cpython/type.pxd",
-  "env/lib/python3.10/site-packages/Cython/Includes/cpython/bool.pxd",
-  "env/lib/python3.10/site-packages/Cython/Includes/cpython/complex.pxd",
+  "env/lib/python3.11/site-packages/Cython/Includes/cpython/type.pxd",
+  "env/lib/python3.11/site-packages/Cython/Includes/cpython/bool.pxd",
+  "env/lib/python3.11/site-packages/Cython/Includes/cpython/complex.pxd",
   "src/_imports.pyx",
   "src/_constants.pyx",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_7pyjson5_Json5Exception;
 struct __pyx_obj_7pyjson5_Json5DecoderException;
@@ -1707,26 +1759,26 @@
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
 
@@ -1780,22 +1832,30 @@
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -2410,22 +2470,22 @@
 static const char __pyx_k_is_not_IOBase_compatible[] = " is not IOBase compatible";
 static const char __pyx_k_src__encoder_options_pyx[] = "src/_encoder_options.pyx";
 static const char __pyx_k_DEFAULT_MAX_NESTING_LEVEL[] = "DEFAULT_MAX_NESTING_LEVEL";
 static const char __pyx_k_Unstringifiable_type_data[] = "Unstringifiable type(data)=";
 static const char __pyx_k_not_in_int_str_bytes_near[] = " not in (int, str, bytes) near ";
 static const char __pyx_k_or_the_value_is_not_valid[] = " or the value is not valid.";
 static const char __pyx_k_Expected_str_instance_or_False[] = "Expected str instance or False";
+static const char __pyx_k_2018_2023_Ren_Kijewski_pypi_org[] = "2018-2023 Ren\303\251 Kijewski <pypi.org@k6i.de>";
 static const char __pyx_k_mappingtypes_must_be_a_sequence[] = "mappingtypes must be a sequence of types or False";
 static const char __pyx_k_quotationmark_must_be_one_ASCII[] = "quotationmark must be one ASCII character.";
 static const char __pyx_k_wordlength_must_be_1_2_or_4_not[] = "wordlength must be 1, 2 or 4, not ";
-static const char __pyx_k_2018_2021_Ren_Kijewski_rene_surn[] = "2018-2021 Ren\303\251 Kijewski <rene.[surname]@fu-berlin.de>";
 static const char __pyx_k_Maximum_nesting_level_exceeded_n[] = "Maximum nesting level exceeded near ";
 static PyObject *__pyx_kp_u_04X;
 static PyObject *__pyx_kp_u_04x;
-static PyObject *__pyx_kp_u_2018_2021_Ren_Kijewski_rene_surn;
+static PyObject *__pyx_kp_u_2018_2023_Ren_Kijewski_pypi_org;
 static PyObject *__pyx_kp_u_47_11;
 static PyObject *__pyx_kp_u_646;
 static PyObject *__pyx_kp_u_8859;
 static PyObject *__pyx_kp_u_Apache_2_0;
 static PyObject *__pyx_n_s_DEFAULT_MAX_NESTING_LEVEL;
 static PyObject *__pyx_n_s_Decimal;
 static PyObject *__pyx_n_s_DecoderException;
@@ -29864,15 +29924,15 @@
   /* "src/_decoder.pyx":525
  * 
  *     c_in_out[0] = c0
  *     return PyUnicode_FromKindAndData(             # <<<<<<<<<<<<<<
  *         PyUnicode_4BYTE_KIND, buf.data(), buf.size(),
  *     )
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(9, 525, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(9, 525, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
   /* "src/_decoder.pyx":486
  * 
  * 
@@ -30226,15 +30286,15 @@
   /* "src/_decoder.pyx":525
  * 
  *     c_in_out[0] = c0
  *     return PyUnicode_FromKindAndData(             # <<<<<<<<<<<<<<
  *         PyUnicode_4BYTE_KIND, buf.data(), buf.size(),
  *     )
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(9, 525, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(9, 525, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
   /* "src/_decoder.pyx":486
  * 
  * 
@@ -30588,15 +30648,15 @@
   /* "src/_decoder.pyx":525
  * 
  *     c_in_out[0] = c0
  *     return PyUnicode_FromKindAndData(             # <<<<<<<<<<<<<<
  *         PyUnicode_4BYTE_KIND, buf.data(), buf.size(),
  *     )
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(9, 525, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(9, 525, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
   /* "src/_decoder.pyx":486
  * 
  * 
@@ -30950,15 +31010,15 @@
   /* "src/_decoder.pyx":525
  * 
  *     c_in_out[0] = c0
  *     return PyUnicode_FromKindAndData(             # <<<<<<<<<<<<<<
  *         PyUnicode_4BYTE_KIND, buf.data(), buf.size(),
  *     )
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(9, 525, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(9, 525, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
   /* "src/_decoder.pyx":486
  * 
  * 
@@ -31312,15 +31372,15 @@
   /* "src/_decoder.pyx":525
  * 
  *     c_in_out[0] = c0
  *     return PyUnicode_FromKindAndData(             # <<<<<<<<<<<<<<
  *         PyUnicode_4BYTE_KIND, buf.data(), buf.size(),
  *     )
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(9, 525, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(9, 525, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
   /* "src/_decoder.pyx":486
  * 
  * 
@@ -49100,15 +49160,15 @@
  * 
  *         self.quotationmark = _options_ascii(quotationmark)             # <<<<<<<<<<<<<<
  *         self.tojson = _options_ascii(tojson, False)
  * 
  */
 __pyx_t_3 = __pyx_f_7pyjson5__options_ascii(__pyx_v_quotationmark, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 122, __pyx_L1_error)
 __Pyx_GOTREF(__pyx_t_3);
-if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(3, 122, __pyx_L1_error)
+if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(3, 122, __pyx_L1_error)
 __Pyx_GIVEREF(__pyx_t_3);
 __Pyx_GOTREF(__pyx_v_self->quotationmark);
 __Pyx_DECREF(__pyx_v_self->quotationmark);
 __pyx_v_self->quotationmark = ((PyObject*)__pyx_t_3);
 __pyx_t_3 = 0;
 
 /* "src/_encoder_options.pyx":123
@@ -49118,15 +49178,15 @@
  * 
  *         if self.quotationmark is None or PyUnicode_GET_LENGTH(self.quotationmark) != 1:
  */
 __pyx_t_4.__pyx_n = 1;
 __pyx_t_4.expect_ascii = 0;
 __pyx_t_3 = __pyx_f_7pyjson5__options_ascii(__pyx_v_tojson, &__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 123, __pyx_L1_error)
 __Pyx_GOTREF(__pyx_t_3);
-if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(3, 123, __pyx_L1_error)
+if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(3, 123, __pyx_L1_error)
 __Pyx_GIVEREF(__pyx_t_3);
 __Pyx_GOTREF(__pyx_v_self->tojson);
 __Pyx_DECREF(__pyx_v_self->tojson);
 __pyx_v_self->tojson = ((PyObject*)__pyx_t_3);
 __pyx_t_3 = 0;
 
 /* "src/_encoder_options.pyx":125
@@ -59060,15 +59120,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
 0, /*tp_vectorcall*/
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
 0, /*tp_print*/
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
 0, /*tp_pypy_flags*/
 #endif
 };
 
 static PyObject *__pyx_tp_new_7pyjson5_Json5DecoderException(PyTypeObject *t, PyObject *a, PyObject *k) {
 PyObject *o = __pyx_tp_new_7pyjson5_Json5Exception(t, a, k);
 if (unlikely(!o)) return 0;
@@ -59151,15 +59211,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
 0, /*tp_vectorcall*/
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
 0, /*tp_print*/
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
 0, /*tp_pypy_flags*/
 #endif
 };
 
 static PyObject *__pyx_tp_new_7pyjson5_Json5NestingTooDeep(PyTypeObject *t, PyObject *a, PyObject *k) {
 PyObject *o = __pyx_tp_new_7pyjson5_Json5DecoderException(t, a, k);
 if (unlikely(!o)) return 0;
@@ -59233,15 +59293,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
 0, /*tp_vectorcall*/
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
 0, /*tp_print*/
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
 0, /*tp_pypy_flags*/
 #endif
 };
 
 static PyObject *__pyx_tp_new_7pyjson5_Json5EOF(PyTypeObject *t, PyObject *a, PyObject *k) {
 PyObject *o = __pyx_tp_new_7pyjson5_Json5DecoderException(t, a, k);
 if (unlikely(!o)) return 0;
@@ -59315,15 +59375,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
 0, /*tp_vectorcall*/
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
 0, /*tp_print*/
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
 0, /*tp_pypy_flags*/
 #endif
 };
 
 static PyObject *__pyx_tp_new_7pyjson5_Json5IllegalCharacter(PyTypeObject *t, PyObject *a, PyObject *k) {
 PyObject *o = __pyx_tp_new_7pyjson5_Json5DecoderException(t, a, k);
 if (unlikely(!o)) return 0;
@@ -59406,15 +59466,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
 0, /*tp_vectorcall*/
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
 0, /*tp_print*/
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
 0, /*tp_pypy_flags*/
 #endif
 };
 
 static PyObject *__pyx_tp_new_7pyjson5_Json5ExtraData(PyTypeObject *t, PyObject *a, PyObject *k) {
 PyObject *o = __pyx_tp_new_7pyjson5_Json5DecoderException(t, a, k);
 if (unlikely(!o)) return 0;
@@ -59497,15 +59557,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
 0, /*tp_vectorcall*/
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
 0, /*tp_print*/
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
 0, /*tp_pypy_flags*/
 #endif
 };
 
 static PyObject *__pyx_tp_new_7pyjson5_Json5IllegalType(PyTypeObject *t, PyObject *a, PyObject *k) {
 PyObject *o = __pyx_tp_new_7pyjson5_Json5DecoderException(t, a, k);
 if (unlikely(!o)) return 0;
@@ -59588,15 +59648,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
 0, /*tp_vectorcall*/
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
 0, /*tp_print*/
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
 0, /*tp_pypy_flags*/
 #endif
 };
 
 static PyObject *__pyx_tp_new_7pyjson5__DecoderException(PyTypeObject *t, PyObject *a, PyObject *k) {
 struct __pyx_obj_7pyjson5__DecoderException *p;
 PyObject *o = (&((PyTypeObject*)PyExc_Exception)[0])->tp_new(t, a, k);
@@ -59729,15 +59789,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
 0, /*tp_vectorcall*/
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
 0, /*tp_print*/
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
 0, /*tp_pypy_flags*/
 #endif
 };
 
 static PyObject *__pyx_tp_new_7pyjson5_Json5EncoderException(PyTypeObject *t, PyObject *a, PyObject *k) {
 PyObject *o = __pyx_tp_new_7pyjson5_Json5Exception(t, a, k);
 if (unlikely(!o)) return 0;
@@ -59811,15 +59871,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
 0, /*tp_vectorcall*/
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
 0, /*tp_print*/
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
 0, /*tp_pypy_flags*/
 #endif
 };
 
 static PyObject *__pyx_tp_new_7pyjson5_Json5UnstringifiableType(PyTypeObject *t, PyObject *a, PyObject *k) {
 PyObject *o = __pyx_tp_new_7pyjson5_Json5EncoderException(t, a, k);
 if (unlikely(!o)) return 0;
@@ -59902,15 +59962,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
 0, /*tp_vectorcall*/
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
 0, /*tp_print*/
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
 0, /*tp_pypy_flags*/
 #endif
 };
 
 static struct __pyx_obj_7pyjson5_Options *__pyx_freelist_7pyjson5_Options[8];
 static int __pyx_freecount_7pyjson5_Options = 0;
 
@@ -60036,15 +60096,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
 0, /*tp_vectorcall*/
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
 0, /*tp_print*/
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
 0, /*tp_pypy_flags*/
 #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
 {0, 0, 0, 0}
 };
@@ -60089,15 +60149,15 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_kp_u_04X, __pyx_k_04X, sizeof(__pyx_k_04X), 0, 1, 0, 0},
   {&__pyx_kp_u_04x, __pyx_k_04x, sizeof(__pyx_k_04x), 0, 1, 0, 0},
-  {&__pyx_kp_u_2018_2021_Ren_Kijewski_rene_surn, __pyx_k_2018_2021_Ren_Kijewski_rene_surn, sizeof(__pyx_k_2018_2021_Ren_Kijewski_rene_surn), 0, 1, 0, 0},
+  {&__pyx_kp_u_2018_2023_Ren_Kijewski_pypi_org, __pyx_k_2018_2023_Ren_Kijewski_pypi_org, sizeof(__pyx_k_2018_2023_Ren_Kijewski_pypi_org), 0, 1, 0, 0},
   {&__pyx_kp_u_47_11, __pyx_k_47_11, sizeof(__pyx_k_47_11), 0, 1, 0, 0},
   {&__pyx_kp_u_646, __pyx_k_646, sizeof(__pyx_k_646), 0, 1, 0, 0},
   {&__pyx_kp_u_8859, __pyx_k_8859, sizeof(__pyx_k_8859), 0, 1, 0, 0},
   {&__pyx_kp_u_Apache_2_0, __pyx_k_Apache_2_0, sizeof(__pyx_k_Apache_2_0), 0, 1, 0, 0},
   {&__pyx_n_s_DEFAULT_MAX_NESTING_LEVEL, __pyx_k_DEFAULT_MAX_NESTING_LEVEL, sizeof(__pyx_k_DEFAULT_MAX_NESTING_LEVEL), 0, 0, 1, 1},
   {&__pyx_n_s_Decimal, __pyx_k_Decimal, sizeof(__pyx_k_Decimal), 0, 0, 1, 1},
   {&__pyx_n_s_DecoderException, __pyx_k_DecoderException, sizeof(__pyx_k_DecoderException), 0, 0, 1, 1},
@@ -60627,15 +60687,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(15, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(15, 1, __pyx_L1_error)
   __pyx_float_0_0 = PyFloat_FromDouble(0.0); if (unlikely(!__pyx_float_0_0)) __PYX_ERR(15, 1, __pyx_L1_error)
   __pyx_float_47_11 = PyFloat_FromDouble(47.11); if (unlikely(!__pyx_float_47_11)) __PYX_ERR(15, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(15, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(15, 1, __pyx_L1_error)
   __pyx_int_32 = PyInt_FromLong(32); if (unlikely(!__pyx_int_32)) __PYX_ERR(15, 1, __pyx_L1_error)
   __pyx_int_646 = PyInt_FromLong(646); if (unlikely(!__pyx_int_646)) __PYX_ERR(15, 1, __pyx_L1_error)
   __pyx_int_4711 = PyInt_FromLong(4711); if (unlikely(!__pyx_int_4711)) __PYX_ERR(15, 1, __pyx_L1_error)
@@ -60829,32 +60889,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(16, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(16, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(16, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(17, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(17, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(17, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(18, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(18, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(18, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -61039,15 +61096,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(15, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(15, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(15, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(15, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(15, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(15, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(15, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_pyjson5) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(15, 1, __pyx_L1_error)
@@ -61628,24 +61685,24 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "src/_exports.pyx":622
  * __doc__ = PyUnicode_FromKindAndData(PyUnicode_1BYTE_KIND, LONGDESCRIPTION, LONGDESCRIPTION_LENGTH)
  * 
  * __license__ = 'Apache-2.0'             # <<<<<<<<<<<<<<
  * 
- * __author__ = '2018-2021 Ren Kijewski <rene.[surname]@fu-berlin.de>'
+ * __author__ = '2018-2023 Ren Kijewski <pypi.org@k6i.de>'
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_license, __pyx_kp_u_Apache_2_0) < 0) __PYX_ERR(13, 622, __pyx_L1_error)
 
   /* "src/_exports.pyx":624
  * __license__ = 'Apache-2.0'
  * 
- * __author__ = '2018-2021 Ren Kijewski <rene.[surname]@fu-berlin.de>'             # <<<<<<<<<<<<<<
+ * __author__ = '2018-2023 Ren Kijewski <pypi.org@k6i.de>'             # <<<<<<<<<<<<<<
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_author, __pyx_kp_u_2018_2021_Ren_Kijewski_rene_surn) < 0) __PYX_ERR(13, 624, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_author, __pyx_kp_u_2018_2023_Ren_Kijewski_pypi_org) < 0) __PYX_ERR(13, 624, __pyx_L1_error)
 
   /* "src/_legacy.pyx":1
  * def loads(s, *, encoding='UTF-8', **kw):             # <<<<<<<<<<<<<<
  *     '''
  *     Decodes JSON5 serialized data from a string.
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7pyjson5_25loads, NULL, __pyx_n_s_pyjson5); if (unlikely(!__pyx_t_2)) __PYX_ERR(14, 1, __pyx_L1_error)
@@ -62318,28 +62375,28 @@
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
@@ -62409,15 +62466,15 @@
         uval = NULL;
         if (uoffset > 0) {
             prepend_sign = !!prepend_sign;
             if (uoffset > prepend_sign) {
                 padding = PyUnicode_FromOrdinal(padding_char);
                 if (likely(padding) && uoffset > prepend_sign + 1) {
                     PyObject *tmp;
-                    PyObject *repeat = PyInt_FromSize_t(uoffset - prepend_sign);
+                    PyObject *repeat = PyInt_FromSsize_t(uoffset - prepend_sign);
                     if (unlikely(!repeat)) goto done_or_error;
                     tmp = PyNumber_Multiply(padding, repeat);
                     Py_DECREF(repeat);
                     Py_DECREF(padding);
                     padding = tmp;
                 }
                 if (unlikely(!padding)) goto done_or_error;
@@ -63121,15 +63178,15 @@
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
@@ -63206,15 +63263,15 @@
     PyObject *r = __Pyx_GetAttr(o, n);
     return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
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
@@ -63325,61 +63382,79 @@
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -63498,15 +63573,15 @@
 #else
     return PyObject_Call((PyObject*)&PyFrozenSet_Type, __pyx_empty_tuple, NULL);
 #endif
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
@@ -63959,15 +64034,15 @@
                         } else if (8 * sizeof(unsigned int) >= 4 * PyLong_SHIFT) {
                             return (unsigned int) (((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -64162,15 +64237,15 @@
                         } else if (8 * sizeof(std::uint32_t) >= 4 * PyLong_SHIFT) {
                             return (std::uint32_t) (((((((((std::uint32_t)digits[3]) << PyLong_SHIFT) | (std::uint32_t)digits[2]) << PyLong_SHIFT) | (std::uint32_t)digits[1]) << PyLong_SHIFT) | (std::uint32_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -64358,15 +64433,15 @@
                         } else if (8 * sizeof(unsigned char) >= 4 * PyLong_SHIFT) {
                             return (unsigned char) (((((((((unsigned char)digits[3]) << PyLong_SHIFT) | (unsigned char)digits[2]) << PyLong_SHIFT) | (unsigned char)digits[1]) << PyLong_SHIFT) | (unsigned char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -64554,15 +64629,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -64750,15 +64825,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -64946,15 +65021,15 @@
                         } else if (8 * sizeof(std::int32_t) >= 4 * PyLong_SHIFT) {
                             return (std::int32_t) (((((((((std::int32_t)digits[3]) << PyLong_SHIFT) | (std::int32_t)digits[2]) << PyLong_SHIFT) | (std::int32_t)digits[1]) << PyLong_SHIFT) | (std::int32_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -65142,15 +65217,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -65338,15 +65413,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `pyjson5-1.6.2/pyjson5.pyx` & `pyjson5-1.6.3/pyjson5.pyx`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # distutils: language = c++
 # cython: embedsignature = True, language_level = 3, warn.undeclared = True, warn.unreachable = True, warn.maybe_uninitialized = True
 
-# Copyright 2018-2021 René Kijewski <rene.SURNAME@fu-berlin.de>
+# Copyright 2018-2023 René Kijewski <pypi.org@k6i.de>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pyjson5-1.6.2/sha512sum.py` & `pyjson5-1.6.3/sha512sum.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,31 +3,33 @@
 from argparse import ArgumentParser
 from hashlib import sha512
 from logging import basicConfig, DEBUG
 from pathlib import Path
 from sys import argv, exit
 
 
-argparser = ArgumentParser(description='sha512sum replacement if coreutils isn\'t installed')
-argparser.add_argument('-c', '--check', type=Path, required=True)
+argparser = ArgumentParser(
+    description="sha512sum replacement if coreutils isn't installed"
+)
+argparser.add_argument("-c", "--check", type=Path, required=True)
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     basicConfig(level=DEBUG)
     args = argparser.parse_args()
     errors = 0
-    with open(str(args.check.resolve()), 'rt') as f:
+    with open(str(args.check.resolve()), "rt") as f:
         for line in f:
-            expected_hash, filename = line.rstrip('\r\n').split('  ', 1)
-            with open(str(Path(filename).resolve()), 'rb') as f:
+            expected_hash, filename = line.rstrip("\r\n").split("  ", 1)
+            with open(str(Path(filename).resolve()), "rb") as f:
                 actual_hash = sha512(f.read()).hexdigest()
 
             if expected_hash == actual_hash:
-                print(filename + ': OK')
+                print(filename + ": OK")
             else:
                 errors += 1
-                print(filename + ': FAILED')
+                print(filename + ": FAILED")
 
     if errors:
-        print('%s: WARNING: %s computed checksum did NOT match' % (argv[0], errors))
+        print("%s: WARNING: %s computed checksum did NOT match" % (argv[0], errors))
         exit(1)
     else:
         exit(0)
```

### Comparing `pyjson5-1.6.2/src/DESCRIPTION.inc` & `pyjson5-1.6.3/src/DESCRIPTION.inc`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_constants.pyx` & `pyjson5-1.6.3/src/_constants.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_decoder.pyx` & `pyjson5-1.6.3/src/_decoder.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_decoder_recursive_select.hpp` & `pyjson5-1.6.3/src/_decoder_recursive_select.hpp`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_encoder.pyx` & `pyjson5-1.6.3/src/_encoder.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_encoder_options.pyx` & `pyjson5-1.6.3/src/_encoder_options.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_escape_dct.hpp` & `pyjson5-1.6.3/src/_escape_dct.hpp`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_exceptions_decoder.pyx` & `pyjson5-1.6.3/src/_exceptions_decoder.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_exceptions_encoder.pyx` & `pyjson5-1.6.3/src/_exceptions_encoder.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_exports.pyx` & `pyjson5-1.6.3/src/_exports.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -617,8 +617,8 @@
     'Json5DecoderException', 'Json5NestingTooDeep', 'Json5EOF', 'Json5IllegalCharacter', 'Json5ExtraData', 'Json5IllegalType',
 )
 
 __doc__ = PyUnicode_FromKindAndData(PyUnicode_1BYTE_KIND, LONGDESCRIPTION, LONGDESCRIPTION_LENGTH)
 
 __license__ = 'Apache-2.0'
 
-__author__ = '2018-2021 René Kijewski <rene.[surname]@fu-berlin.de>'
+__author__ = '2018-2023 René Kijewski <pypi.org@k6i.de>'
```

### Comparing `pyjson5-1.6.2/src/_imports.pyx` & `pyjson5-1.6.3/src/_imports.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_legacy.pyx` & `pyjson5-1.6.3/src/_legacy.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_raise_decoder.pyx` & `pyjson5-1.6.3/src/_raise_decoder.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_reader_callback.pyx` & `pyjson5-1.6.3/src/_reader_callback.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_reader_ucs.pyx` & `pyjson5-1.6.3/src/_reader_ucs.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_readers.pyx` & `pyjson5-1.6.3/src/_readers.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_stack_heap_string.hpp` & `pyjson5-1.6.3/src/_stack_heap_string.hpp`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_unicode.pyx` & `pyjson5-1.6.3/src/_unicode.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_unicode_cat_of.hpp` & `pyjson5-1.6.3/src/_unicode_cat_of.hpp`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_writer_callback.pyx` & `pyjson5-1.6.3/src/_writer_callback.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/_writer_reallocatable.pyx` & `pyjson5-1.6.3/src/_writer_reallocatable.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/dragonbox.cc` & `pyjson5-1.6.3/src/dragonbox.cc`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/native.hpp` & `pyjson5-1.6.3/src/native.hpp`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/src/pyjson5/__init__.pyi` & `pyjson5-1.6.3/src/pyjson5/__init__.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,305 +1,294 @@
 from typing import (
-    Any, Callable, final, Final, Generic, Iterable, Literal, Optional,
-    overload, Protocol, Tuple, TypeVar, Union,
+    Any,
+    Callable,
+    final,
+    Final,
+    Iterable,
+    Literal,
+    Optional,
+    overload,
+    Protocol,
+    Tuple,
+    TypeVar,
+    Union,
 )
 
-
-_T = TypeVar('_T')
+_Data = TypeVar("_Data")
 
 class _SupportsRead(Protocol):
-    def read(self, size: int = ...) -> str:
-        ...
-
-class _SupportsWrite(Generic[_T]):
-    def write(self, s: _T) -> None:
-        ...
+    def read(self, size: int = ...) -> str: ...
 
-_CallbackStr = TypeVar('_CallbackStr', bound=Callable[[str], None])
+class _SupportsWrite(Protocol[_Data]):
+    def write(self, s: _Data) -> Any: ...
 
-_CallbackBytes = TypeVar('_CallbackBytes', bound=Callable[[bytes], None])
+_CallbackStr = TypeVar("_CallbackStr", bound=Callable[[str], None])
 
-_SupportsWriteBytes = TypeVar('_SupportsWriteBytes', bound=_SupportsWrite[bytes])
+_CallbackBytes = TypeVar("_CallbackBytes", bound=Callable[[bytes], None])
 
-_SupportsWriteStr = TypeVar('_SupportsWriteStr', bound=_SupportsWrite[str])
+_SupportsWriteBytes = TypeVar("_SupportsWriteBytes", bound=_SupportsWrite[bytes])
 
+_SupportsWriteStr = TypeVar("_SupportsWriteStr", bound=_SupportsWrite[str])
 
 ###############################################################################
 ### _exports.pyx
 ###############################################################################
 
-
 @final
 class Options:
-    '''Customizations for the ``encoder_*(...)`` function family.'''
+    """Customizations for the ``encoder_*(...)`` function family."""
+
     quotationmark: Final[str] = ...
     tojson: Final[Optional[str]] = ...
     mappingtypes: Final[Tuple[type, ...]] = ...
 
     def __init__(
-        self, *,
+        self,
+        *,
         quotationmark: Optional[str] = ...,
         tojson: Optional[str],
         mappingtypes: Optional[Tuple[type, ...]],
-    ) -> None:
-        ...
-
+    ) -> None: ...
     def update(
-        self, *,
+        self,
+        *,
         quotationmark: Optional[str] = ...,
         tojson: Optional[str],
         mappingtypes: Optional[Tuple[type, ...]],
     ) -> Options:
-        '''Creates a new Options instance by modifying some members.'''
-        ...
+        """Creates a new Options instance by modifying some members."""
 
 def decode(data: str, maxdepth: Optional[int] = ..., some: bool = ...) -> Any:
-    '''Decodes JSON5 serialized data from an ``str`` object.'''
-    ...
+    """Decodes JSON5 serialized data from an ``str`` object."""
 
 def decode_latin1(
-    data: bytes, maxdepth: Optional[int] = ..., some: bool = ...,
+    data: bytes,
+    maxdepth: Optional[int] = ...,
+    some: bool = ...,
 ) -> Any:
-    '''Decodes JSON5 serialized data from a ``bytes`` object.'''
-    ...
+    """Decodes JSON5 serialized data from a ``bytes`` object."""
 
 def decode_utf8(
-    data: bytes, maxdepth: Optional[int] = ..., some: bool = ...,
+    data: bytes,
+    maxdepth: Optional[int] = ...,
+    some: bool = ...,
 ) -> Any:
-    '''Decodes JSON5 serialized data from a ``bytes`` object.'''
-    ...
+    """Decodes JSON5 serialized data from a ``bytes`` object."""
 
 def decode_buffer(
     data: bytes,
     maxdepth: Optional[int] = ...,
     some: bool = ...,
     wordlength: Optional[int] = ...,
 ) -> Any:
-    '''Decodes JSON5 serialized data from an object that supports the buffer protocol, e.g. bytearray.'''
-    ...
+    """Decodes JSON5 serialized data from an object that supports the buffer protocol, e.g. bytearray."""
 
 def decode_callback(
     cb: Callable[..., Union[str, bytes, bytearray, int, None]],
     maxdepth: Optional[int] = ...,
     some: bool = ...,
     args: Optional[Iterable[Any]] = [],
 ) -> Any:
-    '''Decodes JSON5 serialized data by invoking a callback.'''
-    ...
+    """Decodes JSON5 serialized data by invoking a callback."""
 
 def decode_io(
-    fp: _SupportsRead, maxdepth: Optional[int] = ..., some: bool = ...,
+    fp: _SupportsRead,
+    maxdepth: Optional[int] = ...,
+    some: bool = ...,
 ) -> Any:
-    '''Decodes JSON5 serialized data from a file-like object.'''
-    ...
+    """Decodes JSON5 serialized data from a file-like object."""
 
 def encode(
-    data: Any, *,
+    data: Any,
+    *,
     options: Optional[Options] = ...,
     quotationmark: Optional[str] = ...,
     tojson: Optional[str],
     mappingtypes: Optional[Tuple[type, ...]],
 ) -> str:
-    '''Serializes a Python object to a JSON5 compatible string.'''
+    """Serializes a Python object to a JSON5 compatible string."""
     ...
 
 def encode_bytes(
-    data: Any, *,
+    data: Any,
+    *,
     options: Optional[Options] = ...,
     quotationmark: Optional[str] = ...,
     tojson: Optional[str],
     mappingtypes: Optional[Tuple[type, ...]],
 ) -> str:
-    '''Serializes a Python object to a JSON5 compatible bytes string.'''
-    ...
+    """Serializes a Python object to a JSON5 compatible bytes string."""
 
 @overload
 def encode_callback(
-    data: Any, cb: _CallbackStr, supply_bytes: Literal[False] = ..., *,
+    data: Any,
+    cb: _CallbackStr,
+    supply_bytes: Literal[False] = ...,
+    *,
     options: Optional[Options] = ...,
     quotationmark: Optional[str] = ...,
     tojson: Optional[str],
     mappingtypes: Optional[Tuple[type, ...]],
 ) -> _CallbackStr:
-    '''Serializes a Python object into a callback function.'''
-    ...
+    """Serializes a Python object into a callback function."""
 
 @overload
 def encode_callback(
-    data: Any, cb: _CallbackBytes, supply_bytes: Literal[True], *,
+    data: Any,
+    cb: _CallbackBytes,
+    supply_bytes: Literal[True],
+    *,
     options: Optional[Options] = ...,
     quotationmark: Optional[str] = ...,
     tojson: Optional[str],
     mappingtypes: Optional[Tuple[type, ...]],
-) -> _CallbackBytes:
-    ...
-
+) -> _CallbackBytes: ...
 @overload
 def encode_io(
-    data: Any, fp: _SupportsWriteBytes, supply_bytes: Literal[True] = ..., *,
+    data: Any,
+    fp: _SupportsWriteBytes,
+    supply_bytes: Literal[True] = ...,
+    *,
     options: Optional[Options] = ...,
     quotationmark: Optional[str] = ...,
     tojson: Optional[str],
     mappingtypes: Optional[Tuple[type, ...]],
 ) -> _SupportsWriteBytes:
-    '''Serializes a Python object into a file-object.'''
-    ...
+    """Serializes a Python object into a file-object."""
 
 @overload
 def encode_io(
-    data: Any, fp: _SupportsWriteStr, supply_bytes: Literal[False], *,
+    data: Any,
+    fp: _SupportsWriteStr,
+    supply_bytes: Literal[False],
+    *,
     options: Optional[Options] = ...,
     quotationmark: Optional[str] = ...,
     tojson: Optional[str],
     mappingtypes: Optional[Tuple[type, ...]],
-) -> _SupportsWriteStr:
-    ...
-
+) -> _SupportsWriteStr: ...
 def encode_noop(
-    data: Any, *,
+    data: Any,
+    *,
     options: Optional[Options] = ...,
     quotationmark: Optional[str] = ...,
     tojson: Optional[str],
     mappingtypes: Optional[Tuple[type, ...]],
 ) -> bool:
-    '''Test if the input is serializable.'''
-    ...
-
+    """Test if the input is serializable."""
 
 ###############################################################################
 ### _legacy.pyx
 ###############################################################################
 
-
 def loads(s: str, *, encoding: str = ...) -> Any:
-    '''Decodes JSON5 serialized data from a string.'''
-    ...
+    """Decodes JSON5 serialized data from a string."""
 
 def load(fp: _SupportsRead) -> Any:
-    '''Decodes JSON5 serialized data from a file-like object.'''
-    ...
+    """Decodes JSON5 serialized data from a file-like object."""
 
 def dumps(obj: Any) -> str:
-    '''Serializes a Python object to a JSON5 compatible string.'''
-    ...
+    """Serializes a Python object to a JSON5 compatible string."""
 
 def dump(obj: Any, fp: _SupportsWrite[str]) -> None:
-    '''Serializes a Python object to a JSON5 compatible string.'''
-    ...
-
+    """Serializes a Python object to a JSON5 compatible string."""
 
 ###############################################################################
 ### _exceptions.pyx
 ###############################################################################
 
-
 class Json5Exception(Exception):
-    '''Base class of any exception thrown by PyJSON5.'''
-
-    def __init__(self, message: Optional[str] = ..., *args: Any) -> None:
-        ...
+    """Base class of any exception thrown by PyJSON5."""
 
+    def __init__(self, message: Optional[str] = ..., *args: Any) -> None: ...
     @property
-    def message(self) -> Optional[str]:
-        ...
-
+    def message(self) -> Optional[str]: ...
 
 ###############################################################################
 ### _exceptions_encoder.pyx
 ###############################################################################
 
-
 class Json5EncoderException(Json5Exception):
-    '''Base class of any exception thrown by the serializer.'''
-    ...
+    """Base class of any exception thrown by the serializer."""
 
 @final
 class Json5UnstringifiableType(Json5EncoderException):
-    '''The encoder was not able to stringify the input, or it was told not to by the supplied ``Options``.'''
-    def __init__(
-        self, message: Optional[str] = ..., unstringifiable: Any = ...,
-    ) -> None:
-        ...
+    """The encoder was not able to stringify the input, or it was told not to by the supplied ``Options``."""
 
+    def __init__(
+        self,
+        message: Optional[str] = ...,
+        unstringifiable: Any = ...,
+    ) -> None: ...
     @property
     def unstringifiable(self) -> Any:
-        '''The value that caused the problem.'''
-        ...
-
+        """The value that caused the problem."""
 
 ###############################################################################
 ### _exceptions_decoder.pyx
 ###############################################################################
 
-
 class Json5DecoderException(Json5Exception):
-    '''Base class of any exception thrown by the parser.'''
-    def __init__(
-        self, message: Optional[str] = ..., result: Any = ..., *args: Any,
-    ) -> None:
-        ...
+    """Base class of any exception thrown by the parser."""
 
+    def __init__(
+        self,
+        message: Optional[str] = ...,
+        result: Any = ...,
+        *args: Any,
+    ) -> None: ...
     @property
     def result(self) -> Any:
-        '''Deserialized data up until now.'''
-        ...
+        """Deserialized data up until now."""
 
 @final
 class Json5NestingTooDeep(Json5DecoderException):
-    '''The maximum nesting level on the input data was exceeded.'''
-    ...
+    """The maximum nesting level on the input data was exceeded."""
 
 @final
 class Json5EOF(Json5DecoderException):
-    '''The input ended prematurely.'''
-    ...
+    """The input ended prematurely."""
 
 @final
 class Json5IllegalCharacter(Json5DecoderException):
-    '''An unexpected character was encountered.'''
+    """An unexpected character was encountered."""
+
     def __init__(
         self,
         message: Optional[str] = ...,
         result: Any = ...,
         character: Optional[str] = ...,
         *args: Any,
-    ) -> None:
-        ...
-
+    ) -> None: ...
     @property
     def character(self) -> Optional[str]:
-        '''Illegal character.'''
-        ...
+        """Illegal character."""
 
 @final
 class Json5ExtraData(Json5DecoderException):
-    '''The input contained extranous data.'''
+    """The input contained extranous data."""
+
     def __init__(
         self,
         message: Optional[str] = ...,
         result: Any = ...,
         character: Optional[str] = ...,
         *args: Any,
-    ) -> None:
-        ...
-
+    ) -> None: ...
     @property
     def character(self) -> Optional[str]:
-        '''Extranous character.'''
-        ...
+        """Extranous character."""
 
 @final
 class Json5IllegalType(Json5DecoderException):
-    '''The user supplied callback function returned illegal data.'''
+    """The user supplied callback function returned illegal data."""
+
     def __init__(
         self,
         message: Optional[str] = ...,
         result: Any = ...,
         value: Optional[Any] = ...,
         *args: Any,
-    ) -> None:
-        ...
-
+    ) -> None: ...
     @property
     def value(self) -> Optional[Any]:
-        '''Value that caused the problem.'''
-        ...
+        """Value that caused the problem."""
```

### Comparing `pyjson5-1.6.2/src/pyjson5.egg-info/SOURCES.txt` & `pyjson5-1.6.3/src/pyjson5.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjson5-1.6.2/third-party/fast_double_parser/include/fast_double_parser.h` & `pyjson5-1.6.3/third-party/fast_double_parser/include/fast_double_parser.h`

 * *Files identical despite different names*

