# Comparing `tmp/PDKMaster-0.9.2.post1.tar.gz` & `tmp/PDKMaster-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PDKMaster-0.9.2.post1.tar", last modified: Mon May 22 11:49:48 2023, max compression
+gzip compressed data, was "PDKMaster-0.9.3.tar", last modified: Sat Jun 24 16:06:49 2023, max compression
```

## Comparing `PDKMaster-0.9.2.post1.tar` & `PDKMaster-0.9.3.tar`

### file list

```diff
@@ -1,171 +1,177 @@
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.922041 PDKMaster-0.9.2.post1/
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.890041 PDKMaster-0.9.2.post1/.ci/
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1069 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/.ci/check-dco.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      155 2022-01-13 16:15:17.000000 PDKMaster-0.9.2.post1/.gitignore
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2183 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/.gitlab-ci.yml
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6586 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/Contributing.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      566 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/LICENSE.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.890041 PDKMaster-0.9.2.post1/LICENSES/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2021-02-28 15:28:15.000000 PDKMaster-0.9.2.post1/LICENSES/agpl-3.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    11358 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/LICENSES/apache-2.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2021-02-28 15:28:15.000000 PDKMaster-0.9.2.post1/LICENSES/cern_ohl_s_v2.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2021-02-28 15:28:15.000000 PDKMaster-0.9.2.post1/LICENSES/gpl-2.0.txt
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.894041 PDKMaster-0.9.2.post1/PDKMaster.egg-info/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9629 2023-05-22 11:49:48.000000 PDKMaster-0.9.2.post1/PDKMaster.egg-info/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3842 2023-05-22 11:49:48.000000 PDKMaster-0.9.2.post1/PDKMaster.egg-info/SOURCES.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-05-22 11:49:48.000000 PDKMaster-0.9.2.post1/PDKMaster.egg-info/dependency_links.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2023-05-22 11:49:48.000000 PDKMaster-0.9.2.post1/PDKMaster.egg-info/requires.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       15 2023-05-22 11:49:48.000000 PDKMaster-0.9.2.post1/PDKMaster.egg-info/top_level.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9629 2023-05-22 11:49:48.922041 PDKMaster-0.9.2.post1/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9155 2023-05-22 08:56:01.000000 PDKMaster-0.9.2.post1/README.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.894041 PDKMaster-0.9.2.post1/ReleaseNotes/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      442 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/ReleaseNotes/v0.1.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1234 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/ReleaseNotes/v0.2.0.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1471 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/ReleaseNotes/v0.3.0.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2547 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/ReleaseNotes/v0.9.0.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.894041 PDKMaster-0.9.2.post1/assura_yaml/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2020-03-11 19:28:52.000000 PDKMaster-0.9.2.post1/assura_yaml/.keepme
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      595 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/checkskill.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       14 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/ci-requirements.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2022-06-14 17:01:59.000000 PDKMaster-0.9.2.post1/dev-requirements.txt
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.894041 PDKMaster-0.9.2.post1/display_yaml/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2020-03-11 19:28:52.000000 PDKMaster-0.9.2.post1/display_yaml/.keepme
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.878041 PDKMaster-0.9.2.post1/docs/
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.898041 PDKMaster-0.9.2.post1/docs/src/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6063 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/docs/src/conf.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      456 2021-07-22 09:01:44.000000 PDKMaster-0.9.2.post1/docs/src/index.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      141 2021-07-22 09:01:44.000000 PDKMaster-0.9.2.post1/docs/src/pdkmaster._util.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      560 2021-07-22 09:01:44.000000 PDKMaster-0.9.2.post1/docs/src/pdkmaster.design.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      443 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/docs/src/pdkmaster.dispatch.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      312 2022-01-13 16:15:17.000000 PDKMaster-0.9.2.post1/docs/src/pdkmaster.io.coriolis.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      462 2022-02-15 17:28:27.000000 PDKMaster-0.9.2.post1/docs/src/pdkmaster.io.klayout.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      934 2021-07-22 09:01:44.000000 PDKMaster-0.9.2.post1/docs/src/pdkmaster.io.parsing.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      318 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/docs/src/pdkmaster.io.pdkmaster.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      262 2022-01-13 16:15:17.000000 PDKMaster-0.9.2.post1/docs/src/pdkmaster.io.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      449 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/docs/src/pdkmaster.io.spice.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      290 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/docs/src/pdkmaster.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1556 2022-01-13 16:15:17.000000 PDKMaster-0.9.2.post1/docs/src/pdkmaster.technology.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3746 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/dodo.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     4469 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/extract_rules.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    26261 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/files.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.898041 PDKMaster-0.9.2.post1/pdkmaster/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      709 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18133 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/_util.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.898041 PDKMaster-0.9.2.post1/pdkmaster/design/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      237 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/design/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6045 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/design/cell.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10199 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/design/circuit.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8637 2023-04-25 12:12:06.000000 PDKMaster-0.9.2.post1/pdkmaster/design/factory.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.902041 PDKMaster-0.9.2.post1/pdkmaster/design/layout/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      664 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/design/layout/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    28468 2023-04-24 09:20:09.000000 PDKMaster-0.9.2.post1/pdkmaster/design/layout/_circuitlayouter.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    48524 2023-04-24 09:20:09.000000 PDKMaster-0.9.2.post1/pdkmaster/design/layout/_primitivelayouter.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3335 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/design/layout/factory_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    22622 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/design/layout/layout_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2887 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/design/library.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2600 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/design/routinggauge.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.902041 PDKMaster-0.9.2.post1/pdkmaster/dispatch/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1375 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/dispatch/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1378 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/dispatch/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1956 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/dispatch/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7326 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/dispatch/primitive.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2803 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/dispatch/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3801 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/dispatch/shape.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.902041 PDKMaster-0.9.2.post1/pdkmaster/io/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.902041 PDKMaster-0.9.2.post1/pdkmaster/io/coriolis/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/coriolis/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    58622 2023-05-22 08:38:12.000000 PDKMaster-0.9.2.post1/pdkmaster/io/coriolis/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.902041 PDKMaster-0.9.2.post1/pdkmaster/io/klayout/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      142 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/klayout/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37892 2023-05-15 14:41:43.000000 PDKMaster-0.9.2.post1/pdkmaster/io/klayout/export.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    23519 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/klayout/merge_.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.906041 PDKMaster-0.9.2.post1/pdkmaster/io/notebook/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      121 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/notebook/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1253 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/notebook/plotter.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.906041 PDKMaster-0.9.2.post1/pdkmaster/io/parsing/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      214 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/parsing/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18847 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/parsing/assura.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      422 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/parsing/display.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      822 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/parsing/layermap.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17548 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/parsing/skill_grammar.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24374 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/parsing/tf.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.906041 PDKMaster-0.9.2.post1/pdkmaster/io/pdkmaster/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/pdkmaster/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18079 2023-04-24 09:20:09.000000 PDKMaster-0.9.2.post1/pdkmaster/io/pdkmaster/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.906041 PDKMaster-0.9.2.post1/pdkmaster/io/spice/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      165 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/spice/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    15809 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/spice/pyspice.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     5904 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/spice/spice_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      181 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/io/spice/typing.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.910041 PDKMaster-0.9.2.post1/pdkmaster/technology/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      276 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4032 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    77846 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/geometry.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17939 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      627 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/net.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.910041 PDKMaster-0.9.2.post1/pdkmaster/technology/primitive/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      466 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/primitive/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9661 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/primitive/_core.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1519 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/primitive/_derived.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1176 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/primitive/_param.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24763 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/primitive/conductors.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    44372 2023-05-19 11:07:45.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/primitive/devices.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4914 2023-05-19 11:07:45.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/primitive/layers.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6752 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/primitive/rules.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9109 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/property_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2138 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20002 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/technology_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2059 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/pdkmaster/technology/wafer_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3224 2023-05-19 14:44:16.000000 PDKMaster-0.9.2.post1/pdkmaster/typing.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-05-22 11:49:48.922041 PDKMaster-0.9.2.post1/setup.cfg
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1410 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/setup.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      863 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/skill.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1278 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/skill2yaml.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.914041 PDKMaster-0.9.2.post1/test/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.914041 PDKMaster-0.9.2.post1/test/unit/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7946 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/_util.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.914041 PDKMaster-0.9.2.post1/test/unit/design/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/design/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3025 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/design/cell.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2470 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/design/circuit.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3664 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/design/factory.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37534 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/design/layout.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4584 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/design/library.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.918041 PDKMaster-0.9.2.post1/test/unit/dispatch/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/dispatch/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1343 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/dispatch/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1397 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/dispatch/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1688 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/dispatch/primitive.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1531 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/dispatch/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3403 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/dispatch/shape.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    12960 2023-04-24 09:20:09.000000 PDKMaster-0.9.2.post1/test/unit/dummy.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.918041 PDKMaster-0.9.2.post1/test/unit/io/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/io/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.918041 PDKMaster-0.9.2.post1/test/unit/io/klayout/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/io/klayout/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13480 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/io/klayout/export.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20839 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/io/klayout/merge.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.918041 PDKMaster-0.9.2.post1/test/unit/io/pdkmaster/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/io/pdkmaster/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1862 2023-04-24 09:20:09.000000 PDKMaster-0.9.2.post1/test/unit/io/pdkmaster/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.918041 PDKMaster-0.9.2.post1/test/unit/io/spice/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/io/spice/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7947 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/io/spice/pyspice.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1317 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/io/spice/spice_.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.922041 PDKMaster-0.9.2.post1/test/unit/technology/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/technology/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1313 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/technology/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    56025 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/technology/geometry.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6112 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/technology/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    53443 2023-04-24 09:20:09.000000 PDKMaster-0.9.2.post1/test/unit/technology/primitive.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2775 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/technology/property.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2072 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/technology/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    12778 2023-04-24 09:20:09.000000 PDKMaster-0.9.2.post1/test/unit/technology/technology.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1052 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/technology/wafer.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1278 2023-04-07 09:59:24.000000 PDKMaster-0.9.2.post1/test/unit/typing.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      673 2020-03-11 19:28:52.000000 PDKMaster-0.9.2.post1/test.tf
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-05-22 11:49:48.922041 PDKMaster-0.9.2.post1/tf_yaml/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2020-03-11 19:28:52.000000 PDKMaster-0.9.2.post1/tf_yaml/.keepme
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.972625 PDKMaster-0.9.3/
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.940625 PDKMaster-0.9.3/.ci/
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1069 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/.ci/check-dco.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      155 2022-01-13 16:15:17.000000 PDKMaster-0.9.3/.gitignore
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2183 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/.gitlab-ci.yml
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6586 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/Contributing.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      566 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/LICENSE.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.940625 PDKMaster-0.9.3/LICENSES/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2021-02-28 15:28:15.000000 PDKMaster-0.9.3/LICENSES/agpl-3.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    11358 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/LICENSES/apache-2.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2021-02-28 15:28:15.000000 PDKMaster-0.9.3/LICENSES/cern_ohl_s_v2.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2021-02-28 15:28:15.000000 PDKMaster-0.9.3/LICENSES/gpl-2.0.txt
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.940625 PDKMaster-0.9.3/PDKMaster.egg-info/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9707 2023-06-24 16:06:49.000000 PDKMaster-0.9.3/PDKMaster.egg-info/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3966 2023-06-24 16:06:49.000000 PDKMaster-0.9.3/PDKMaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-06-24 16:06:49.000000 PDKMaster-0.9.3/PDKMaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2023-06-24 16:06:49.000000 PDKMaster-0.9.3/PDKMaster.egg-info/requires.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       15 2023-06-24 16:06:49.000000 PDKMaster-0.9.3/PDKMaster.egg-info/top_level.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9707 2023-06-24 16:06:49.972625 PDKMaster-0.9.3/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9239 2023-06-24 15:43:31.000000 PDKMaster-0.9.3/README.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.940625 PDKMaster-0.9.3/ReleaseNotes/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      442 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/ReleaseNotes/v0.1.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1234 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/ReleaseNotes/v0.2.0.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1471 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/ReleaseNotes/v0.3.0.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2547 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/ReleaseNotes/v0.9.0.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.944625 PDKMaster-0.9.3/assura_yaml/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2020-03-11 19:28:52.000000 PDKMaster-0.9.3/assura_yaml/.keepme
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      595 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/checkskill.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       14 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/ci-requirements.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2022-06-14 17:01:59.000000 PDKMaster-0.9.3/dev-requirements.txt
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.944625 PDKMaster-0.9.3/display_yaml/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2020-03-11 19:28:52.000000 PDKMaster-0.9.3/display_yaml/.keepme
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.932624 PDKMaster-0.9.3/docs/
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.944625 PDKMaster-0.9.3/docs/src/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6063 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/docs/src/conf.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      456 2021-07-22 09:01:44.000000 PDKMaster-0.9.3/docs/src/index.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      141 2021-07-22 09:01:44.000000 PDKMaster-0.9.3/docs/src/pdkmaster._util.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      560 2021-07-22 09:01:44.000000 PDKMaster-0.9.3/docs/src/pdkmaster.design.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      443 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/docs/src/pdkmaster.dispatch.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      312 2022-01-13 16:15:17.000000 PDKMaster-0.9.3/docs/src/pdkmaster.io.coriolis.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      462 2022-02-15 17:28:27.000000 PDKMaster-0.9.3/docs/src/pdkmaster.io.klayout.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      934 2021-07-22 09:01:44.000000 PDKMaster-0.9.3/docs/src/pdkmaster.io.parsing.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      318 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/docs/src/pdkmaster.io.pdkmaster.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      262 2022-01-13 16:15:17.000000 PDKMaster-0.9.3/docs/src/pdkmaster.io.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      449 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/docs/src/pdkmaster.io.spice.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      290 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/docs/src/pdkmaster.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1556 2022-01-13 16:15:17.000000 PDKMaster-0.9.3/docs/src/pdkmaster.technology.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3746 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/dodo.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     4469 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/extract_rules.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    26261 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/files.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.948624 PDKMaster-0.9.3/pdkmaster/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      709 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18133 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/_util.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.948624 PDKMaster-0.9.3/pdkmaster/design/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      237 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/design/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6045 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/design/cell.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10199 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/design/circuit.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8637 2023-04-25 12:12:06.000000 PDKMaster-0.9.3/pdkmaster/design/factory.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.948624 PDKMaster-0.9.3/pdkmaster/design/layout/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      664 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/design/layout/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    28610 2023-06-02 15:47:08.000000 PDKMaster-0.9.3/pdkmaster/design/layout/_circuitlayouter.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    48524 2023-05-26 16:05:30.000000 PDKMaster-0.9.3/pdkmaster/design/layout/_primitivelayouter.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3335 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/design/layout/factory_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    22622 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/design/layout/layout_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2887 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/design/library.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2600 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/design/routinggauge.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.952625 PDKMaster-0.9.3/pdkmaster/dispatch/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1375 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/dispatch/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1378 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/dispatch/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1956 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/dispatch/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7326 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/dispatch/primitive.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2803 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/dispatch/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3801 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/dispatch/shape.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.952625 PDKMaster-0.9.3/pdkmaster/io/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.952625 PDKMaster-0.9.3/pdkmaster/io/coriolis/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/coriolis/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    58622 2023-05-30 07:56:45.000000 PDKMaster-0.9.3/pdkmaster/io/coriolis/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.952625 PDKMaster-0.9.3/pdkmaster/io/klayout/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      142 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/klayout/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37892 2023-05-26 16:05:30.000000 PDKMaster-0.9.3/pdkmaster/io/klayout/export.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    23519 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/klayout/merge_.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.952625 PDKMaster-0.9.3/pdkmaster/io/lefdef/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      261 2023-05-30 07:56:45.000000 PDKMaster-0.9.3/pdkmaster/io/lefdef/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9950 2023-05-30 07:56:45.000000 PDKMaster-0.9.3/pdkmaster/io/lefdef/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.952625 PDKMaster-0.9.3/pdkmaster/io/notebook/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      121 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/notebook/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1253 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/notebook/plotter.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.956625 PDKMaster-0.9.3/pdkmaster/io/parsing/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      214 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/parsing/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18847 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/parsing/assura.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      422 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/parsing/display.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      822 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/parsing/layermap.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17548 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/parsing/skill_grammar.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24374 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/parsing/tf.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.956625 PDKMaster-0.9.3/pdkmaster/io/pdkmaster/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/pdkmaster/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18079 2023-05-26 16:05:30.000000 PDKMaster-0.9.3/pdkmaster/io/pdkmaster/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.956625 PDKMaster-0.9.3/pdkmaster/io/spice/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      165 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/spice/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    15809 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/spice/pyspice.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     5904 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/spice/spice_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      181 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/spice/typing.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.960625 PDKMaster-0.9.3/pdkmaster/technology/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      276 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4032 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    77846 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/geometry.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17939 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      627 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/net.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.960625 PDKMaster-0.9.3/pdkmaster/technology/primitive/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      466 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/primitive/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9661 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/primitive/_core.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1519 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/primitive/_derived.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1176 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/primitive/_param.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24763 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/primitive/conductors.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    44372 2023-05-30 07:56:57.000000 PDKMaster-0.9.3/pdkmaster/technology/primitive/devices.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4914 2023-05-30 07:56:57.000000 PDKMaster-0.9.3/pdkmaster/technology/primitive/layers.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6752 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/primitive/rules.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9109 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/property_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2138 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20002 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/technology_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2059 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/wafer_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3224 2023-05-30 07:56:45.000000 PDKMaster-0.9.3/pdkmaster/typing.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-06-24 16:06:49.972625 PDKMaster-0.9.3/setup.cfg
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1410 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/setup.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      863 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/skill.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1278 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/skill2yaml.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.960625 PDKMaster-0.9.3/test/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.964625 PDKMaster-0.9.3/test/unit/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7946 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/_util.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.964625 PDKMaster-0.9.3/test/unit/design/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/design/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3025 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/design/cell.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2470 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/design/circuit.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3664 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/design/factory.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37534 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/design/layout.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4584 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/design/library.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.964625 PDKMaster-0.9.3/test/unit/dispatch/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/dispatch/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1343 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/dispatch/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1397 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/dispatch/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1688 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/dispatch/primitive.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1531 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/dispatch/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3403 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/dispatch/shape.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13091 2023-05-30 07:56:45.000000 PDKMaster-0.9.3/test/unit/dummy.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.964625 PDKMaster-0.9.3/test/unit/io/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/io/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.968625 PDKMaster-0.9.3/test/unit/io/klayout/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/io/klayout/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13480 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/io/klayout/export.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20839 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/io/klayout/merge.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.968625 PDKMaster-0.9.3/test/unit/io/lefdef/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-05-30 07:56:45.000000 PDKMaster-0.9.3/test/unit/io/lefdef/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1573 2023-05-30 07:56:45.000000 PDKMaster-0.9.3/test/unit/io/lefdef/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.968625 PDKMaster-0.9.3/test/unit/io/pdkmaster/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/io/pdkmaster/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1862 2023-05-26 16:05:30.000000 PDKMaster-0.9.3/test/unit/io/pdkmaster/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.968625 PDKMaster-0.9.3/test/unit/io/spice/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/io/spice/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7947 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/io/spice/pyspice.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1317 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/io/spice/spice_.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.972625 PDKMaster-0.9.3/test/unit/technology/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/technology/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1313 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/technology/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    56025 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/technology/geometry.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6112 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/technology/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    53443 2023-05-26 16:05:30.000000 PDKMaster-0.9.3/test/unit/technology/primitive.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2775 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/technology/property.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2072 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/technology/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    12778 2023-05-26 16:05:30.000000 PDKMaster-0.9.3/test/unit/technology/technology.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1052 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/technology/wafer.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1278 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/typing.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      673 2020-03-11 19:28:52.000000 PDKMaster-0.9.3/test.tf
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.972625 PDKMaster-0.9.3/tf_yaml/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2020-03-11 19:28:52.000000 PDKMaster-0.9.3/tf_yaml/.keepme
```

### Comparing `PDKMaster-0.9.2.post1/.ci/check-dco.py` & `PDKMaster-0.9.3/.ci/check-dco.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/.gitlab-ci.yml` & `PDKMaster-0.9.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/Contributing.md` & `PDKMaster-0.9.3/Contributing.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/LICENSE.md` & `PDKMaster-0.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/LICENSES/agpl-3.0.txt` & `PDKMaster-0.9.3/LICENSES/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/LICENSES/apache-2.0.txt` & `PDKMaster-0.9.3/LICENSES/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/LICENSES/cern_ohl_s_v2.txt` & `PDKMaster-0.9.3/LICENSES/cern_ohl_s_v2.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/LICENSES/gpl-2.0.txt` & `PDKMaster-0.9.3/LICENSES/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/PDKMaster.egg-info/PKG-INFO` & `PDKMaster-0.9.3/PDKMaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDKMaster
-Version: 0.9.2.post1
+Version: 0.9.3
 Summary: ASIC PDK Manager and Design Framework
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: AGPL-3.0-or-later OR GPL-2.0-or-later OR CERN-OHL-S-2.0+ OR Apache-2.0
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/PDKMaster
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/PDKMaster/issues
 Requires-Python: >=3.6
@@ -14,14 +14,17 @@
 # Description
 
 PDK Master is a tool to manage [PDK](https://en.wikipedia.org/wiki/Process_design_kit)s for ASIC design and a framework for designing circuits and layouts in those technologies.
 It is a Python framework under heavy development and with an unstable API.
 
 # Release history
 
+* v0.9.3:
+  * First LEF/DEF support: support exporting tech.lef file
+  * Bug fixing
 * v0.9.2: support new namespace in coriolis export
 * v0.9.1: fix coriolis export, primitive type values are not python types.
 * v0.9.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md)
 * v0.3.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.3.0/ReleaseNotes/v0.3.0.md)
 * v0.2.1: add klayout dependency
 * v0.2.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.2.0/ReleaseNotes/v0.2.0.md)
 * v0.1: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.2.0/ReleaseNotes/v0.1.md)
```

### Comparing `PDKMaster-0.9.2.post1/PDKMaster.egg-info/SOURCES.txt` & `PDKMaster-0.9.3/PDKMaster.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,16 @@
 pdkmaster/dispatch/shape.py
 pdkmaster/io/__init__.py
 pdkmaster/io/coriolis/__init__.py
 pdkmaster/io/coriolis/export.py
 pdkmaster/io/klayout/__init__.py
 pdkmaster/io/klayout/export.py
 pdkmaster/io/klayout/merge_.py
+pdkmaster/io/lefdef/__init__.py
+pdkmaster/io/lefdef/export.py
 pdkmaster/io/notebook/__init__.py
 pdkmaster/io/notebook/plotter.py
 pdkmaster/io/parsing/__init__.py
 pdkmaster/io/parsing/assura.py
 pdkmaster/io/parsing/display.py
 pdkmaster/io/parsing/layermap.py
 pdkmaster/io/parsing/skill_grammar.py
@@ -116,14 +118,16 @@
 test/unit/dispatch/primitive.py
 test/unit/dispatch/rule.py
 test/unit/dispatch/shape.py
 test/unit/io/__init__.py
 test/unit/io/klayout/__init__.py
 test/unit/io/klayout/export.py
 test/unit/io/klayout/merge.py
+test/unit/io/lefdef/__init__.py
+test/unit/io/lefdef/export.py
 test/unit/io/pdkmaster/__init__.py
 test/unit/io/pdkmaster/export.py
 test/unit/io/spice/__init__.py
 test/unit/io/spice/pyspice.py
 test/unit/io/spice/spice_.py
 test/unit/technology/__init__.py
 test/unit/technology/edge.py
```

### Comparing `PDKMaster-0.9.2.post1/PKG-INFO` & `PDKMaster-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDKMaster
-Version: 0.9.2.post1
+Version: 0.9.3
 Summary: ASIC PDK Manager and Design Framework
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: AGPL-3.0-or-later OR GPL-2.0-or-later OR CERN-OHL-S-2.0+ OR Apache-2.0
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/PDKMaster
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/PDKMaster/issues
 Requires-Python: >=3.6
@@ -14,14 +14,17 @@
 # Description
 
 PDK Master is a tool to manage [PDK](https://en.wikipedia.org/wiki/Process_design_kit)s for ASIC design and a framework for designing circuits and layouts in those technologies.
 It is a Python framework under heavy development and with an unstable API.
 
 # Release history
 
+* v0.9.3:
+  * First LEF/DEF support: support exporting tech.lef file
+  * Bug fixing
 * v0.9.2: support new namespace in coriolis export
 * v0.9.1: fix coriolis export, primitive type values are not python types.
 * v0.9.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md)
 * v0.3.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.3.0/ReleaseNotes/v0.3.0.md)
 * v0.2.1: add klayout dependency
 * v0.2.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.2.0/ReleaseNotes/v0.2.0.md)
 * v0.1: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.2.0/ReleaseNotes/v0.1.md)
```

### Comparing `PDKMaster-0.9.2.post1/README.md` & `PDKMaster-0.9.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Description
 
 PDK Master is a tool to manage [PDK](https://en.wikipedia.org/wiki/Process_design_kit)s for ASIC design and a framework for designing circuits and layouts in those technologies.
 It is a Python framework under heavy development and with an unstable API.
 
 # Release history
 
+* v0.9.3:
+  * First LEF/DEF support: support exporting tech.lef file
+  * Bug fixing
 * v0.9.2: support new namespace in coriolis export
 * v0.9.1: fix coriolis export, primitive type values are not python types.
 * v0.9.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md)
 * v0.3.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.3.0/ReleaseNotes/v0.3.0.md)
 * v0.2.1: add klayout dependency
 * v0.2.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.2.0/ReleaseNotes/v0.2.0.md)
 * v0.1: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.2.0/ReleaseNotes/v0.1.md)
```

### Comparing `PDKMaster-0.9.2.post1/ReleaseNotes/v0.2.0.md` & `PDKMaster-0.9.3/ReleaseNotes/v0.2.0.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/ReleaseNotes/v0.3.0.md` & `PDKMaster-0.9.3/ReleaseNotes/v0.3.0.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/ReleaseNotes/v0.9.0.md` & `PDKMaster-0.9.3/ReleaseNotes/v0.9.0.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/checkskill.py` & `PDKMaster-0.9.3/checkskill.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/docs/src/conf.py` & `PDKMaster-0.9.3/docs/src/conf.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/docs/src/pdkmaster.design.rst` & `PDKMaster-0.9.3/docs/src/pdkmaster.design.rst`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/docs/src/pdkmaster.io.parsing.rst` & `PDKMaster-0.9.3/docs/src/pdkmaster.io.parsing.rst`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/docs/src/pdkmaster.technology.rst` & `PDKMaster-0.9.3/docs/src/pdkmaster.technology.rst`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/dodo.py` & `PDKMaster-0.9.3/dodo.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/extract_rules.py` & `PDKMaster-0.9.3/extract_rules.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/files.py` & `PDKMaster-0.9.3/files.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/__init__.py` & `PDKMaster-0.9.3/pdkmaster/__init__.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/_util.py` & `PDKMaster-0.9.3/pdkmaster/_util.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/design/cell.py` & `PDKMaster-0.9.3/pdkmaster/design/cell.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/design/circuit.py` & `PDKMaster-0.9.3/pdkmaster/design/circuit.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/design/factory.py` & `PDKMaster-0.9.3/pdkmaster/design/factory.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/design/layout/__init__.py` & `PDKMaster-0.9.3/pdkmaster/design/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/design/layout/_circuitlayouter.py` & `PDKMaster-0.9.3/pdkmaster/design/layout/_circuitlayouter.py`

 * *Files 0% similar despite different names*

```diff
@@ -687,14 +687,16 @@
         if bottom_top is not None:
             shape = _geo.Rect.from_rect(rect=shape, top=bottom_top)
             draw = True
         if draw:
             kwargs = {}
             if "bottom_implant" in via_params:
                 kwargs["implant"] = via_params["bottom_implant"]
+            if "bottom_implant_enclosure" in via_params:
+                kwargs["implant_enclosure"] = via_params["bottom_implant_enclosure"]
             if "bottom_well" in via_params:
                 kwargs["well"] = via_params["bottom_well"]
                 kwargs["well_net"] = via_params["well_net"]
             l = self.add_wire(wire=bottom, net=net, shape=shape, **kwargs)
             via_lay += l
 
         return via_lay
```

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/design/layout/_primitivelayouter.py` & `PDKMaster-0.9.3/pdkmaster/design/layout/_primitivelayouter.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/design/layout/factory_.py` & `PDKMaster-0.9.3/pdkmaster/design/layout/factory_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/design/layout/layout_.py` & `PDKMaster-0.9.3/pdkmaster/design/layout/layout_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/design/library.py` & `PDKMaster-0.9.3/pdkmaster/design/library.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/design/routinggauge.py` & `PDKMaster-0.9.3/pdkmaster/design/routinggauge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/dispatch/__init__.py` & `PDKMaster-0.9.3/pdkmaster/dispatch/__init__.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/dispatch/edge.py` & `PDKMaster-0.9.3/pdkmaster/dispatch/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/dispatch/mask.py` & `PDKMaster-0.9.3/pdkmaster/dispatch/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/dispatch/primitive.py` & `PDKMaster-0.9.3/pdkmaster/dispatch/primitive.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/dispatch/rule.py` & `PDKMaster-0.9.3/pdkmaster/dispatch/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/dispatch/shape.py` & `PDKMaster-0.9.3/pdkmaster/dispatch/shape.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/io/coriolis/export.py` & `PDKMaster-0.9.3/pdkmaster/io/coriolis/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/io/klayout/export.py` & `PDKMaster-0.9.3/pdkmaster/io/klayout/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/io/klayout/merge_.py` & `PDKMaster-0.9.3/pdkmaster/io/klayout/merge_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/io/notebook/plotter.py` & `PDKMaster-0.9.3/pdkmaster/io/notebook/plotter.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/io/parsing/assura.py` & `PDKMaster-0.9.3/pdkmaster/io/parsing/assura.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/io/parsing/layermap.py` & `PDKMaster-0.9.3/pdkmaster/io/parsing/layermap.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/io/parsing/skill_grammar.py` & `PDKMaster-0.9.3/pdkmaster/io/parsing/skill_grammar.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/io/parsing/tf.py` & `PDKMaster-0.9.3/pdkmaster/io/parsing/tf.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/io/pdkmaster/export.py` & `PDKMaster-0.9.3/pdkmaster/io/pdkmaster/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/io/spice/pyspice.py` & `PDKMaster-0.9.3/pdkmaster/io/spice/pyspice.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/io/spice/spice_.py` & `PDKMaster-0.9.3/pdkmaster/io/spice/spice_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/technology/edge.py` & `PDKMaster-0.9.3/pdkmaster/technology/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/technology/geometry.py` & `PDKMaster-0.9.3/pdkmaster/technology/geometry.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/technology/mask.py` & `PDKMaster-0.9.3/pdkmaster/technology/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/technology/net.py` & `PDKMaster-0.9.3/pdkmaster/technology/net.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/technology/primitive/_core.py` & `PDKMaster-0.9.3/pdkmaster/technology/primitive/_core.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/technology/primitive/_derived.py` & `PDKMaster-0.9.3/pdkmaster/technology/primitive/_derived.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/technology/primitive/_param.py` & `PDKMaster-0.9.3/pdkmaster/technology/primitive/_param.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/technology/primitive/conductors.py` & `PDKMaster-0.9.3/pdkmaster/technology/primitive/conductors.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/technology/primitive/devices.py` & `PDKMaster-0.9.3/pdkmaster/technology/primitive/devices.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/technology/primitive/layers.py` & `PDKMaster-0.9.3/pdkmaster/technology/primitive/layers.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/technology/primitive/rules.py` & `PDKMaster-0.9.3/pdkmaster/technology/primitive/rules.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/technology/property_.py` & `PDKMaster-0.9.3/pdkmaster/technology/property_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/technology/rule.py` & `PDKMaster-0.9.3/pdkmaster/technology/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/technology/technology_.py` & `PDKMaster-0.9.3/pdkmaster/technology/technology_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/technology/wafer_.py` & `PDKMaster-0.9.3/pdkmaster/technology/wafer_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/pdkmaster/typing.py` & `PDKMaster-0.9.3/pdkmaster/typing.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/setup.py` & `PDKMaster-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/skill.py` & `PDKMaster-0.9.3/skill.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/skill2yaml.py` & `PDKMaster-0.9.3/skill2yaml.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/_util.py` & `PDKMaster-0.9.3/test/unit/_util.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/design/cell.py` & `PDKMaster-0.9.3/test/unit/design/cell.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/design/circuit.py` & `PDKMaster-0.9.3/test/unit/design/circuit.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/design/factory.py` & `PDKMaster-0.9.3/test/unit/design/factory.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/design/layout.py` & `PDKMaster-0.9.3/test/unit/design/layout.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/design/library.py` & `PDKMaster-0.9.3/test/unit/design/library.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/dispatch/edge.py` & `PDKMaster-0.9.3/test/unit/dispatch/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/dispatch/mask.py` & `PDKMaster-0.9.3/test/unit/dispatch/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/dispatch/primitive.py` & `PDKMaster-0.9.3/test/unit/dispatch/primitive.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/dispatch/rule.py` & `PDKMaster-0.9.3/test/unit/dispatch/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/dispatch/shape.py` & `PDKMaster-0.9.3/test/unit/dispatch/shape.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/dummy.py` & `PDKMaster-0.9.3/test/unit/dummy.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,34 +42,36 @@
         prims = _prm.Primitives(_prm.Base(type_=_prm.nBase))
 
         nwell = _prm.Well(type_=_prm.nImpl, name="nwell", min_width=1.5, min_space=1.5)
         deepwell = _prm.DeepWell(
             name="deepwell", min_width=3.0, min_space=3.0,
             well=nwell, min_well_overlap=0.8, min_well_enclosure=0.8,
         )
+        pwell = _prm.Well(type_=_prm.pImpl, name="pwell", min_width=1.5, min_space=1.5)
         nplus = _prm.Implant(type_=_prm.nImpl, name="nplus", min_width=1.0, min_space=1.0)
         pplus = _prm.Implant(type_=_prm.pImpl, name="pplus", min_width=1.0, min_space=1.0)
         hvox = _prm.Insulator(name="hvox", min_width=0.5, min_space=0.5)
         active = _prm.WaferWire(
             name="active", min_width=0.3, min_space=0.2,
             allow_in_substrate=True,
             implant=(nplus, pplus), min_implant_enclosure=_prp.Enclosure(0.2),
             implant_abut="none", allow_contactless_implant=False,
-            well=nwell, min_well_enclosure=_prp.Enclosure(1.0),
+            well=(nwell, pwell), min_well_enclosure=_prp.Enclosure(1.0),
             min_substrate_enclosure=_prp.Enclosure(1.0),
             oxide=hvox, min_oxide_enclosure=_prp.Enclosure(0.2),
             allow_well_crossing=False,
         )
         poly = _prm.GateWire(name="poly", min_width=0.25, min_space=0.25)
-        prims += (nwell, deepwell, nplus, pplus, hvox, active, poly)
+        prims += (nwell, deepwell, pwell, nplus, pplus, hvox, active, poly)
 
         metalpin = _prm.Marker(name="metalpin")
         metal = _prm.MetalWire(
             name="metal",
-            min_width=0.1, min_space=0.1, space_table=({0.2, 0.5},), min_density=0.20,
+            min_width=0.1, min_space=0.1, space_table=({0.2, 0.5},), min_area=0.05,
+            min_density=0.20,
             pin=metalpin,
         )
         contact = _prm.Via(
             name="contact", width=0.35, min_space=0.35, bottom=(active, poly), top=metal,
             min_bottom_enclosure=_prp.Enclosure(0.2), min_top_enclosure=_prp.Enclosure(0.15),
         )
         prims += (contact, metalpin, metal)
```

### Comparing `PDKMaster-0.9.2.post1/test/unit/io/klayout/export.py` & `PDKMaster-0.9.3/test/unit/io/klayout/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/io/klayout/merge.py` & `PDKMaster-0.9.3/test/unit/io/klayout/merge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/io/pdkmaster/export.py` & `PDKMaster-0.9.3/test/unit/io/pdkmaster/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/io/spice/pyspice.py` & `PDKMaster-0.9.3/test/unit/io/spice/pyspice.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/io/spice/spice_.py` & `PDKMaster-0.9.3/test/unit/io/spice/spice_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/technology/edge.py` & `PDKMaster-0.9.3/test/unit/technology/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/technology/geometry.py` & `PDKMaster-0.9.3/test/unit/technology/geometry.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/technology/mask.py` & `PDKMaster-0.9.3/test/unit/technology/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/technology/primitive.py` & `PDKMaster-0.9.3/test/unit/technology/primitive.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/technology/property.py` & `PDKMaster-0.9.3/test/unit/technology/property.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/technology/rule.py` & `PDKMaster-0.9.3/test/unit/technology/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/technology/technology.py` & `PDKMaster-0.9.3/test/unit/technology/technology.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/technology/wafer.py` & `PDKMaster-0.9.3/test/unit/technology/wafer.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test/unit/typing.py` & `PDKMaster-0.9.3/test/unit/typing.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.2.post1/test.tf` & `PDKMaster-0.9.3/test.tf`

 * *Files identical despite different names*

