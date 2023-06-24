# Comparing `tmp/no_vtf-3.0.0.tar.gz` & `tmp/no_vtf-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "no_vtf-3.0.0.tar", last modified: Fri Jun  9 18:24:31 2023, max compression
+gzip compressed data, was "no_vtf-3.0.1.tar", last modified: Sat Jun 24 10:20:05 2023, max compression
```

## Comparing `no_vtf-3.0.0.tar` & `no_vtf-3.0.1.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.554766 no_vtf-3.0.0/
--rw-r--r--   0 build     (1000) build     (1000)     1726 2023-06-09 18:14:25.000000 no_vtf-3.0.0/.build.yml
--rw-r--r--   0 build     (1000) build     (1000)      336 2023-06-09 18:14:25.000000 no_vtf-3.0.0/.gitignore
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.534767 no_vtf-3.0.0/.reuse/
--rw-r--r--   0 build     (1000) build     (1000)      189 2023-06-09 18:14:25.000000 no_vtf-3.0.0/.reuse/dep5
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.538767 no_vtf-3.0.0/LICENSES/
--rw-r--r--   0 build     (1000) build     (1000)    17023 2023-06-09 18:14:25.000000 no_vtf-3.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 build     (1000) build     (1000)     7048 2023-06-09 18:14:25.000000 no_vtf-3.0.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 build     (1000) build     (1000)    34670 2023-06-09 18:14:25.000000 no_vtf-3.0.0/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 build     (1000) build     (1000)    42098 2023-06-09 18:14:25.000000 no_vtf-3.0.0/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 build     (1000) build     (1000)      138 2023-06-09 18:14:25.000000 no_vtf-3.0.0/MANIFEST.in
--rw-r--r--   0 build     (1000) build     (1000)     9026 2023-06-09 18:24:31.554766 no_vtf-3.0.0/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1000)     7738 2023-06-09 18:14:25.000000 no_vtf-3.0.0/README.md
--rw-r--r--   0 build     (1000) build     (1000)       95 2023-06-09 18:14:25.000000 no_vtf-3.0.0/README.md.license
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.538767 no_vtf-3.0.0/builds/
--rw-r--r--   0 build     (1000) build     (1000)      820 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/common
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.538767 no_vtf-3.0.0/builds/debian/
--rw-r--r--   0 build     (1000) build     (1000)      162 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/debian/common
--rwxr-xr-x   0 build     (1000) build     (1000)      401 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/debian/env.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      404 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/debian/ksc-install.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      508 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/debian/python3.10-build_dep.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      855 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/debian/wine-install.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      180 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/diff_generated.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      188 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/nox.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      198 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/nox_wine.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      466 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/python3.10-install.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      363 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/verify_signatures.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      264 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/with_clone.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      989 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/with_wine.sh
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.538767 no_vtf-3.0.0/ksy/
--rwxr-xr-x   0 build     (1000) build     (1000)      205 2023-06-09 18:14:25.000000 no_vtf-3.0.0/ksy/compile.sh
--rw-r--r--   0 build     (1000) build     (1000)    10409 2023-06-09 18:14:25.000000 no_vtf-3.0.0/ksy/vtf.ksy
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.542766 no_vtf-3.0.0/no_vtf/
--rw-r--r--   0 build     (1000) build     (1000)      329 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      300 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/__main__.py
--rw-r--r--   0 build     (1000) build     (1000)      160 2023-06-09 18:24:31.000000 no_vtf-3.0.0/no_vtf/_version.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.542766 no_vtf-3.0.0/no_vtf/deferred/
--rw-r--r--   0 build     (1000) build     (1000)      186 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/deferred/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1471 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/deferred/deferred.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.542766 no_vtf-3.0.0/no_vtf/filesystem/
--rw-r--r--   0 build     (1000) build     (1000)      287 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/filesystem/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     2023 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/filesystem/input_paths.py
--rw-r--r--   0 build     (1000) build     (1000)      895 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/filesystem/output_directories.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.546766 no_vtf-3.0.0/no_vtf/image/
--rw-r--r--   0 build     (1000) build     (1000)      441 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1667 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/channel_separator.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.546766 no_vtf-3.0.0/no_vtf/image/decoder/
--rw-r--r--   0 build     (1000) build     (1000)      198 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/decoder/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      486 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/decoder/decoder.py
--rw-r--r--   0 build     (1000) build     (1000)     7697 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/decoder/generic.py
--rw-r--r--   0 build     (1000) build     (1000)     2797 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/decoder/vtf.py
--rw-r--r--   0 build     (1000) build     (1000)     1497 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/image.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.546766 no_vtf-3.0.0/no_vtf/image/modifier/
--rw-r--r--   0 build     (1000) build     (1000)      202 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/modifier/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1632 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/modifier/fp_precision_modifier.py
--rw-r--r--   0 build     (1000) build     (1000)      540 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/modifier/modifier.py
--rw-r--r--   0 build     (1000) build     (1000)      946 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/ndarray.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.546766 no_vtf-3.0.0/no_vtf/io/
--rw-r--r--   0 build     (1000) build     (1000)      264 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/io/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      573 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/io/bytes.py
--rw-r--r--   0 build     (1000) build     (1000)     7977 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/io/image.py
--rw-r--r--   0 build     (1000) build     (1000)      933 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/io/io.py
--rw-r--r--   0 build     (1000) build     (1000)    11149 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/main.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.546766 no_vtf-3.0.0/no_vtf/parser/
--rw-r--r--   0 build     (1000) build     (1000)        0 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/parser/__init__.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.546766 no_vtf-3.0.0/no_vtf/parser/generated/
--rw-r--r--   0 build     (1000) build     (1000)        0 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/parser/generated/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)    25192 2023-06-09 18:24:12.000000 no_vtf-3.0.0/no_vtf/parser/generated/vtf.py
--rw-r--r--   0 build     (1000) build     (1000)       93 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/parser/generated/vtf.py.license
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.546766 no_vtf-3.0.0/no_vtf/pipeline/
--rw-r--r--   0 build     (1000) build     (1000)      186 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/pipeline/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     4936 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/pipeline/pipeline.py
--rw-r--r--   0 build     (1000) build     (1000)        0 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/py.typed
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.550766 no_vtf-3.0.0/no_vtf/task_runner/
--rw-r--r--   0 build     (1000) build     (1000)      356 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/task_runner/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1524 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/task_runner/parallel.py
--rw-r--r--   0 build     (1000) build     (1000)      826 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/task_runner/sequential.py
--rw-r--r--   0 build     (1000) build     (1000)     1085 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/task_runner/task_runner.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.550766 no_vtf-3.0.0/no_vtf/texture/
--rw-r--r--   0 build     (1000) build     (1000)        0 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/__init__.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.550766 no_vtf-3.0.0/no_vtf/texture/decoder/
--rw-r--r--   0 build     (1000) build     (1000)      204 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/decoder/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      486 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/decoder/decoder.py
--rw-r--r--   0 build     (1000) build     (1000)     4485 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/decoder/vtf.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.550766 no_vtf-3.0.0/no_vtf/texture/extractor/
--rw-r--r--   0 build     (1000) build     (1000)      212 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/extractor/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      453 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/extractor/extractor.py
--rw-r--r--   0 build     (1000) build     (1000)     4010 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/extractor/vtf.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.550766 no_vtf-3.0.0/no_vtf/texture/filter/
--rw-r--r--   0 build     (1000) build     (1000)      200 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/filter/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      367 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/filter/filter.py
--rw-r--r--   0 build     (1000) build     (1000)     2756 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/filter/vtf.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.550766 no_vtf-3.0.0/no_vtf/texture/namer/
--rw-r--r--   0 build     (1000) build     (1000)      196 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/namer/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      374 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/namer/namer.py
--rw-r--r--   0 build     (1000) build     (1000)     1025 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/namer/vtf.py
--rw-r--r--   0 build     (1000) build     (1000)      663 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/vtf.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.542766 no_vtf-3.0.0/no_vtf.egg-info/
--rw-r--r--   0 build     (1000) build     (1000)     9026 2023-06-09 18:24:31.000000 no_vtf-3.0.0/no_vtf.egg-info/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1000)     2409 2023-06-09 18:24:31.000000 no_vtf-3.0.0/no_vtf.egg-info/SOURCES.txt
--rw-r--r--   0 build     (1000) build     (1000)        1 2023-06-09 18:24:31.000000 no_vtf-3.0.0/no_vtf.egg-info/dependency_links.txt
--rw-r--r--   0 build     (1000) build     (1000)       49 2023-06-09 18:24:31.000000 no_vtf-3.0.0/no_vtf.egg-info/entry_points.txt
--rw-r--r--   0 build     (1000) build     (1000)        1 2023-06-09 18:23:29.000000 no_vtf-3.0.0/no_vtf.egg-info/not-zip-safe
--rw-r--r--   0 build     (1000) build     (1000)      183 2023-06-09 18:24:31.000000 no_vtf-3.0.0/no_vtf.egg-info/requires.txt
--rw-r--r--   0 build     (1000) build     (1000)        7 2023-06-09 18:24:31.000000 no_vtf-3.0.0/no_vtf.egg-info/top_level.txt
--rw-r--r--   0 build     (1000) build     (1000)     9785 2023-06-09 18:14:25.000000 no_vtf-3.0.0/noxfile.py
--rw-r--r--   0 build     (1000) build     (1000)      682 2023-06-09 18:14:25.000000 no_vtf-3.0.0/pyproject.toml
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.534767 no_vtf-3.0.0/resources/
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.550766 no_vtf-3.0.0/resources/docs/
--rw-r--r--   0 build     (1000) build     (1000)   123671 2023-06-09 18:14:25.000000 no_vtf-3.0.0/resources/docs/screencast.gif
--rw-r--r--   0 build     (1000) build     (1000)       95 2023-06-09 18:14:25.000000 no_vtf-3.0.0/resources/docs/screencast.gif.license
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.554766 no_vtf-3.0.0/resources/pyinstaller/
--rw-r--r--   0 build     (1000) build     (1000)        6 2023-06-09 18:14:25.000000 no_vtf-3.0.0/resources/pyinstaller/empty.ico
--rw-r--r--   0 build     (1000) build     (1000)       93 2023-06-09 18:14:25.000000 no_vtf-3.0.0/resources/pyinstaller/empty.ico.license
--rwxr-xr-x   0 build     (1000) build     (1000)      276 2023-06-09 18:14:25.000000 no_vtf-3.0.0/resources/pyinstaller/no_vtf.desktop
--rw-r--r--   0 build     (1000) build     (1000)      103 2023-06-09 18:14:25.000000 no_vtf-3.0.0/resources/pyinstaller/no_vtf.desktop.license
--rw-r--r--   0 build     (1000) build     (1000)     2657 2023-06-09 18:24:31.554766 no_vtf-3.0.0/setup.cfg
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.137010 no_vtf-3.0.1/
+-rw-r--r--   0 build     (1000) build     (1000)     1655 2023-06-24 10:09:58.000000 no_vtf-3.0.1/.build.yml
+-rw-r--r--   0 build     (1000) build     (1000)      336 2023-06-24 10:09:58.000000 no_vtf-3.0.1/.gitignore
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.121010 no_vtf-3.0.1/.reuse/
+-rw-r--r--   0 build     (1000) build     (1000)      189 2023-06-24 10:09:58.000000 no_vtf-3.0.1/.reuse/dep5
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.121010 no_vtf-3.0.1/LICENSES/
+-rw-r--r--   0 build     (1000) build     (1000)    17023 2023-06-24 10:09:58.000000 no_vtf-3.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 build     (1000) build     (1000)     7048 2023-06-24 10:09:58.000000 no_vtf-3.0.1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 build     (1000) build     (1000)    34670 2023-06-24 10:09:58.000000 no_vtf-3.0.1/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 build     (1000) build     (1000)    42098 2023-06-24 10:09:58.000000 no_vtf-3.0.1/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 build     (1000) build     (1000)      138 2023-06-24 10:09:58.000000 no_vtf-3.0.1/MANIFEST.in
+-rw-r--r--   0 build     (1000) build     (1000)     9540 2023-06-24 10:20:05.137010 no_vtf-3.0.1/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1000)     8269 2023-06-24 10:09:58.000000 no_vtf-3.0.1/README.md
+-rw-r--r--   0 build     (1000) build     (1000)       95 2023-06-24 10:09:58.000000 no_vtf-3.0.1/README.md.license
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.125010 no_vtf-3.0.1/builds/
+-rw-r--r--   0 build     (1000) build     (1000)      559 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/common
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.125010 no_vtf-3.0.1/builds/debian/
+-rw-r--r--   0 build     (1000) build     (1000)      162 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/debian/common
+-rwxr-xr-x   0 build     (1000) build     (1000)      401 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/debian/env.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      404 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/debian/ksc-install.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      510 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/debian/python3.10-build_dep.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      855 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/debian/wine-install.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      180 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/diff_generated.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      188 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/nox.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      198 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/nox_wine.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      641 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/publish_frozen.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      466 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/python3.10-install.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      363 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/verify_signatures.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      264 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/with_clone.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      989 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/with_wine.sh
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.125010 no_vtf-3.0.1/ksy/
+-rwxr-xr-x   0 build     (1000) build     (1000)      205 2023-06-24 10:09:58.000000 no_vtf-3.0.1/ksy/compile.sh
+-rw-r--r--   0 build     (1000) build     (1000)    10409 2023-06-24 10:09:58.000000 no_vtf-3.0.1/ksy/vtf.ksy
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.125010 no_vtf-3.0.1/no_vtf/
+-rw-r--r--   0 build     (1000) build     (1000)      329 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      300 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/__main__.py
+-rw-r--r--   0 build     (1000) build     (1000)      160 2023-06-24 10:20:04.000000 no_vtf-3.0.1/no_vtf/_version.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.129010 no_vtf-3.0.1/no_vtf/deferred/
+-rw-r--r--   0 build     (1000) build     (1000)      186 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/deferred/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1471 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/deferred/deferred.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.129010 no_vtf-3.0.1/no_vtf/filesystem/
+-rw-r--r--   0 build     (1000) build     (1000)      287 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/filesystem/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     2023 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/filesystem/input_paths.py
+-rw-r--r--   0 build     (1000) build     (1000)      895 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/filesystem/output_directories.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.129010 no_vtf-3.0.1/no_vtf/image/
+-rw-r--r--   0 build     (1000) build     (1000)      441 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1667 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/channel_separator.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.129010 no_vtf-3.0.1/no_vtf/image/decoder/
+-rw-r--r--   0 build     (1000) build     (1000)      198 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/decoder/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      486 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/decoder/decoder.py
+-rw-r--r--   0 build     (1000) build     (1000)     7697 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/decoder/generic.py
+-rw-r--r--   0 build     (1000) build     (1000)     2797 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/decoder/vtf.py
+-rw-r--r--   0 build     (1000) build     (1000)     1497 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/image.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.133010 no_vtf-3.0.1/no_vtf/image/modifier/
+-rw-r--r--   0 build     (1000) build     (1000)      202 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/modifier/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1632 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/modifier/fp_precision_modifier.py
+-rw-r--r--   0 build     (1000) build     (1000)      540 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/modifier/modifier.py
+-rw-r--r--   0 build     (1000) build     (1000)      946 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/ndarray.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.133010 no_vtf-3.0.1/no_vtf/io/
+-rw-r--r--   0 build     (1000) build     (1000)      264 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/io/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      573 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/io/bytes.py
+-rw-r--r--   0 build     (1000) build     (1000)     7976 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/io/image.py
+-rw-r--r--   0 build     (1000) build     (1000)      933 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/io/io.py
+-rw-r--r--   0 build     (1000) build     (1000)    11148 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/main.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.133010 no_vtf-3.0.1/no_vtf/parser/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/parser/__init__.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.133010 no_vtf-3.0.1/no_vtf/parser/generated/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/parser/generated/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)    25192 2023-06-24 10:19:46.000000 no_vtf-3.0.1/no_vtf/parser/generated/vtf.py
+-rw-r--r--   0 build     (1000) build     (1000)       93 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/parser/generated/vtf.py.license
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.133010 no_vtf-3.0.1/no_vtf/pipeline/
+-rw-r--r--   0 build     (1000) build     (1000)      186 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/pipeline/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     4935 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/pipeline/pipeline.py
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/py.typed
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.133010 no_vtf-3.0.1/no_vtf/task_runner/
+-rw-r--r--   0 build     (1000) build     (1000)      356 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/task_runner/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1524 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/task_runner/parallel.py
+-rw-r--r--   0 build     (1000) build     (1000)      826 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/task_runner/sequential.py
+-rw-r--r--   0 build     (1000) build     (1000)     1085 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/task_runner/task_runner.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.133010 no_vtf-3.0.1/no_vtf/texture/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/__init__.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.133010 no_vtf-3.0.1/no_vtf/texture/decoder/
+-rw-r--r--   0 build     (1000) build     (1000)      204 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/decoder/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      486 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/decoder/decoder.py
+-rw-r--r--   0 build     (1000) build     (1000)     4485 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/decoder/vtf.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.137010 no_vtf-3.0.1/no_vtf/texture/extractor/
+-rw-r--r--   0 build     (1000) build     (1000)      212 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/extractor/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      453 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/extractor/extractor.py
+-rw-r--r--   0 build     (1000) build     (1000)     4010 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/extractor/vtf.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.137010 no_vtf-3.0.1/no_vtf/texture/filter/
+-rw-r--r--   0 build     (1000) build     (1000)      200 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/texture/filter/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      367 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/texture/filter/filter.py
+-rw-r--r--   0 build     (1000) build     (1000)     2756 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/texture/filter/vtf.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.137010 no_vtf-3.0.1/no_vtf/texture/namer/
+-rw-r--r--   0 build     (1000) build     (1000)      196 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/namer/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      374 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/namer/namer.py
+-rw-r--r--   0 build     (1000) build     (1000)     1025 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/texture/namer/vtf.py
+-rw-r--r--   0 build     (1000) build     (1000)      663 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/vtf.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.129010 no_vtf-3.0.1/no_vtf.egg-info/
+-rw-r--r--   0 build     (1000) build     (1000)     9540 2023-06-24 10:20:04.000000 no_vtf-3.0.1/no_vtf.egg-info/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1000)     2434 2023-06-24 10:20:05.000000 no_vtf-3.0.1/no_vtf.egg-info/SOURCES.txt
+-rw-r--r--   0 build     (1000) build     (1000)        1 2023-06-24 10:20:04.000000 no_vtf-3.0.1/no_vtf.egg-info/dependency_links.txt
+-rw-r--r--   0 build     (1000) build     (1000)       49 2023-06-24 10:20:04.000000 no_vtf-3.0.1/no_vtf.egg-info/entry_points.txt
+-rw-r--r--   0 build     (1000) build     (1000)        1 2023-06-24 10:19:06.000000 no_vtf-3.0.1/no_vtf.egg-info/not-zip-safe
+-rw-r--r--   0 build     (1000) build     (1000)      183 2023-06-24 10:20:04.000000 no_vtf-3.0.1/no_vtf.egg-info/requires.txt
+-rw-r--r--   0 build     (1000) build     (1000)        7 2023-06-24 10:20:04.000000 no_vtf-3.0.1/no_vtf.egg-info/top_level.txt
+-rw-r--r--   0 build     (1000) build     (1000)     9785 2023-06-24 10:09:58.000000 no_vtf-3.0.1/noxfile.py
+-rw-r--r--   0 build     (1000) build     (1000)      682 2023-06-24 10:09:58.000000 no_vtf-3.0.1/pyproject.toml
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.121010 no_vtf-3.0.1/resources/
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.137010 no_vtf-3.0.1/resources/docs/
+-rw-r--r--   0 build     (1000) build     (1000)   123671 2023-06-24 10:09:58.000000 no_vtf-3.0.1/resources/docs/screencast.gif
+-rw-r--r--   0 build     (1000) build     (1000)       95 2023-06-24 10:09:58.000000 no_vtf-3.0.1/resources/docs/screencast.gif.license
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.137010 no_vtf-3.0.1/resources/pyinstaller/
+-rw-r--r--   0 build     (1000) build     (1000)        6 2023-06-24 10:09:58.000000 no_vtf-3.0.1/resources/pyinstaller/empty.ico
+-rw-r--r--   0 build     (1000) build     (1000)       93 2023-06-24 10:09:58.000000 no_vtf-3.0.1/resources/pyinstaller/empty.ico.license
+-rwxr-xr-x   0 build     (1000) build     (1000)      276 2023-06-24 10:09:58.000000 no_vtf-3.0.1/resources/pyinstaller/no_vtf.desktop
+-rw-r--r--   0 build     (1000) build     (1000)      103 2023-06-24 10:09:58.000000 no_vtf-3.0.1/resources/pyinstaller/no_vtf.desktop.license
+-rw-r--r--   0 build     (1000) build     (1000)     2640 2023-06-24 10:20:05.141010 no_vtf-3.0.1/setup.cfg
```

### Comparing `no_vtf-3.0.0/.build.yml` & `no_vtf-3.0.1/.build.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-image: debian/stable
+image: debian/bullseye
 arch: amd64
 
 secrets:
 - a3cafe86-e4dd-4f18-b7ad-5809c8d577f2
 - 076fcca6-4239-4488-bf29-ec6dd1e9852c
 
 oauth: pages.sr.ht/PAGES:RW
@@ -39,31 +39,34 @@
       builds/debian/ksc-install.sh
       builds/diff_generated.sh
 
   - package: |
       cd no_vtf
       builds/nox.sh --session package -- ~/no_vtf.tar.gz
 
+  - package_wine: |
+      cd no_vtf
+      builds/with_wine.sh /tmp/wine builds/with_clone.sh builds/nox_wine.sh --session package
+
   - freeze: |
       cd no_vtf
       builds/with_clone.sh builds/nox.sh --session freeze -- ~/no_vtf-linux_x64.tar.xz
 
   - freeze_wine: |
       cd no_vtf
       builds/with_wine.sh /tmp/wine builds/with_clone.sh builds/nox_wine.sh --session freeze -- ~/no_vtf-windows_x64.zip
 
   - verify_signatures: |
       cd no_vtf
       builds/verify_signatures.sh || complete-build
 
   - pre-release: |
       cd no_vtf
-      [ "$(git rev-parse --verify HEAD)" == "$(git rev-parse --verify master)" ] || complete-build
       git describe --exact-match 2>/dev/null || complete-build
 
   - publish_frozen: |
-      tar czf release.tar.gz no_vtf-linux_x64.tar.xz no_vtf-windows_x64.zip
-      acurl --no-progress-meter --form content=@release.tar.gz https://pages.sr.ht/publish/b5327157.srht.site/no_vtf/release
+      cd no_vtf
+      builds/publish_frozen.sh ~ no_vtf-linux_x64.tar.xz no_vtf-windows_x64.zip
 
   - publish_package: |
       cd no_vtf
       builds/nox.sh --session publish -- ~/.pypi.org.token
```

### Comparing `no_vtf-3.0.0/LICENSES/CC-BY-4.0.txt` & `no_vtf-3.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/LICENSES/CC0-1.0.txt` & `no_vtf-3.0.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/LICENSES/GPL-3.0-or-later.txt` & `no_vtf-3.0.1/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/LICENSES/LGPL-3.0-or-later.txt` & `no_vtf-3.0.1/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/PKG-INFO` & `no_vtf-3.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: no_vtf
-Version: 3.0.0
+Version: 3.0.1
 Summary: Valve Texture Format Converter
 Home-page: https://sr.ht/~b5327157/no_vtf
 Author: b5327157
 Author-email: b5327157@protonmail.com
-License: GNU Lesser General Public License v3 or later (LGPLv3+)
+License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Download, https://sr.ht/~b5327157/no_vtf/#application-bundle
 Project-URL: Changelog, https://git.sr.ht/~b5327157/no_vtf/refs
 Project-URL: Mailing list, https://lists.sr.ht/~b5327157/no_vtf
 Project-URL: Ticket tracker, https://todo.sr.ht/~b5327157/no_vtf
 Project-URL: Wiki, https://developer.valvesoftware.com/wiki/no_vtf
 Keywords: Source Engine,VTF,Valve Texture Format
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-License-File: LICENSES/LGPL-3.0-or-later.txt
+License-File: LICENSES/GPL-3.0-or-later.txt
 
 # no_vtf
 
 Say no to [.vtf](https://developer.valvesoftware.com/wiki/Valve_Texture_Format) – convert it to one of the standard image formats.
 
 ![Badge showing supported Python versions](https://img.shields.io/pypi/pyversions/no_vtf?style=flat-square)
 [![Badge showing package version on PyPI](https://img.shields.io/pypi/v/no_vtf?style=flat-square)](https://pypi.org/project/no-vtf/)
@@ -226,7 +226,11 @@
 ### Pre-build steps
 
 ```
 # compile .ksy files (requires Kaitai Struct compiler)
 # only necessary if a .ksy file was modified
 ksy/compile.sh
 ```
+
+## License
+
+The package is licensed under [GNU LGPL v3.0 or later](https://spdx.org/licenses/LGPL-3.0-or-later.html), except of image IO done with the help of the [ImageIO FreeImage](https://github.com/imageio/imageio-freeimage) plugin. This makes the entire package effectively licensed under [GNU GPL v3.0 or later](https://spdx.org/licenses/GPL-3.0-or-later.html). If you make use of the image IO part (either directly or indirectly) when linking to no_vtf as a library, the combined work is licensed under the latter license.
```

### Comparing `no_vtf-3.0.0/README.md` & `no_vtf-3.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -197,7 +197,11 @@
 ### Pre-build steps
 
 ```
 # compile .ksy files (requires Kaitai Struct compiler)
 # only necessary if a .ksy file was modified
 ksy/compile.sh
 ```
+
+## License
+
+The package is licensed under [GNU LGPL v3.0 or later](https://spdx.org/licenses/LGPL-3.0-or-later.html), except of image IO done with the help of the [ImageIO FreeImage](https://github.com/imageio/imageio-freeimage) plugin. This makes the entire package effectively licensed under [GNU GPL v3.0 or later](https://spdx.org/licenses/GPL-3.0-or-later.html). If you make use of the image IO part (either directly or indirectly) when linking to no_vtf as a library, the combined work is licensed under the latter license.
```

### Comparing `no_vtf-3.0.0/builds/debian/wine-install.sh` & `no_vtf-3.0.1/builds/debian/wine-install.sh`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/builds/with_wine.sh` & `no_vtf-3.0.1/builds/with_wine.sh`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/ksy/vtf.ksy` & `no_vtf-3.0.1/ksy/vtf.ksy`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/deferred/deferred.py` & `no_vtf-3.0.1/no_vtf/deferred/deferred.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/filesystem/input_paths.py` & `no_vtf-3.0.1/no_vtf/filesystem/input_paths.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/filesystem/output_directories.py` & `no_vtf-3.0.1/no_vtf/filesystem/output_directories.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/image/channel_separator.py` & `no_vtf-3.0.1/no_vtf/image/channel_separator.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/image/decoder/generic.py` & `no_vtf-3.0.1/no_vtf/image/decoder/generic.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/image/decoder/vtf.py` & `no_vtf-3.0.1/no_vtf/image/decoder/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/image/image.py` & `no_vtf-3.0.1/no_vtf/image/image.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/image/modifier/fp_precision_modifier.py` & `no_vtf-3.0.1/no_vtf/image/modifier/fp_precision_modifier.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/image/modifier/modifier.py` & `no_vtf-3.0.1/no_vtf/image/modifier/modifier.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/image/ndarray.py` & `no_vtf-3.0.1/no_vtf/image/ndarray.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/io/bytes.py` & `no_vtf-3.0.1/no_vtf/io/bytes.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/io/image.py` & `no_vtf-3.0.1/no_vtf/io/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
 #
-# SPDX-License-Identifier: LGPL-3.0-or-later
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 from __future__ import annotations
 
 import functools
 import pathlib
 import re
```

### Comparing `no_vtf-3.0.0/no_vtf/io/io.py` & `no_vtf-3.0.1/no_vtf/io/io.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/main.py` & `no_vtf-3.0.1/no_vtf/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
 #
-# SPDX-License-Identifier: LGPL-3.0-or-later
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 from __future__ import annotations
 
 import contextlib
 import inspect
 import pathlib
 import re
```

### Comparing `no_vtf-3.0.0/no_vtf/parser/generated/vtf.py` & `no_vtf-3.0.1/no_vtf/parser/generated/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/pipeline/pipeline.py` & `no_vtf-3.0.1/no_vtf/pipeline/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
 #
-# SPDX-License-Identifier: LGPL-3.0-or-later
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 from __future__ import annotations
 
 import pathlib
 import re
 
 from dataclasses import dataclass
```

### Comparing `no_vtf-3.0.0/no_vtf/task_runner/parallel.py` & `no_vtf-3.0.1/no_vtf/task_runner/parallel.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/task_runner/sequential.py` & `no_vtf-3.0.1/no_vtf/task_runner/sequential.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/task_runner/task_runner.py` & `no_vtf-3.0.1/no_vtf/task_runner/task_runner.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/texture/decoder/vtf.py` & `no_vtf-3.0.1/no_vtf/texture/decoder/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/texture/extractor/vtf.py` & `no_vtf-3.0.1/no_vtf/texture/extractor/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/texture/filter/vtf.py` & `no_vtf-3.0.1/no_vtf/texture/filter/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/texture/namer/vtf.py` & `no_vtf-3.0.1/no_vtf/texture/namer/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf/texture/vtf.py` & `no_vtf-3.0.1/no_vtf/texture/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/no_vtf.egg-info/PKG-INFO` & `no_vtf-3.0.1/no_vtf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: no-vtf
-Version: 3.0.0
+Version: 3.0.1
 Summary: Valve Texture Format Converter
 Home-page: https://sr.ht/~b5327157/no_vtf
 Author: b5327157
 Author-email: b5327157@protonmail.com
-License: GNU Lesser General Public License v3 or later (LGPLv3+)
+License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Download, https://sr.ht/~b5327157/no_vtf/#application-bundle
 Project-URL: Changelog, https://git.sr.ht/~b5327157/no_vtf/refs
 Project-URL: Mailing list, https://lists.sr.ht/~b5327157/no_vtf
 Project-URL: Ticket tracker, https://todo.sr.ht/~b5327157/no_vtf
 Project-URL: Wiki, https://developer.valvesoftware.com/wiki/no_vtf
 Keywords: Source Engine,VTF,Valve Texture Format
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-License-File: LICENSES/LGPL-3.0-or-later.txt
+License-File: LICENSES/GPL-3.0-or-later.txt
 
 # no_vtf
 
 Say no to [.vtf](https://developer.valvesoftware.com/wiki/Valve_Texture_Format) – convert it to one of the standard image formats.
 
 ![Badge showing supported Python versions](https://img.shields.io/pypi/pyversions/no_vtf?style=flat-square)
 [![Badge showing package version on PyPI](https://img.shields.io/pypi/v/no_vtf?style=flat-square)](https://pypi.org/project/no-vtf/)
@@ -226,7 +226,11 @@
 ### Pre-build steps
 
 ```
 # compile .ksy files (requires Kaitai Struct compiler)
 # only necessary if a .ksy file was modified
 ksy/compile.sh
 ```
+
+## License
+
+The package is licensed under [GNU LGPL v3.0 or later](https://spdx.org/licenses/LGPL-3.0-or-later.html), except of image IO done with the help of the [ImageIO FreeImage](https://github.com/imageio/imageio-freeimage) plugin. This makes the entire package effectively licensed under [GNU GPL v3.0 or later](https://spdx.org/licenses/GPL-3.0-or-later.html). If you make use of the image IO part (either directly or indirectly) when linking to no_vtf as a library, the combined work is licensed under the latter license.
```

### Comparing `no_vtf-3.0.0/no_vtf.egg-info/SOURCES.txt` & `no_vtf-3.0.1/no_vtf.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 LICENSES/CC0-1.0.txt
 LICENSES/GPL-3.0-or-later.txt
 LICENSES/LGPL-3.0-or-later.txt
 builds/common
 builds/diff_generated.sh
 builds/nox.sh
 builds/nox_wine.sh
+builds/publish_frozen.sh
 builds/python3.10-install.sh
 builds/verify_signatures.sh
 builds/with_clone.sh
 builds/with_wine.sh
 builds/debian/common
 builds/debian/env.sh
 builds/debian/ksc-install.sh
```

### Comparing `no_vtf-3.0.0/noxfile.py` & `no_vtf-3.0.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/pyproject.toml` & `no_vtf-3.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/resources/docs/screencast.gif` & `no_vtf-3.0.1/resources/docs/screencast.gif`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.0/setup.cfg` & `no_vtf-3.0.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [metadata]
 author = b5327157
 author_email = b5327157@protonmail.com
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: End Users/Desktop
-	License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Topic :: Multimedia :: Graphics :: Graphics Conversion
 	Typing :: Typed
 description = Valve Texture Format Converter
 keywords = 
 	Source Engine
 	VTF
 	Valve Texture Format
-license = GNU Lesser General Public License v3 or later (LGPLv3+)
+license = GNU General Public License v3 or later (GPLv3+)
 license_files = 
-	LICENSES/LGPL-3.0-or-later.txt
+	LICENSES/GPL-3.0-or-later.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = no_vtf
 project_urls = 
 	Download = https://sr.ht/~b5327157/no_vtf/#application-bundle
 	Changelog = https://git.sr.ht/~b5327157/no_vtf/refs
 	Mailing list = https://lists.sr.ht/~b5327157/no_vtf
```

