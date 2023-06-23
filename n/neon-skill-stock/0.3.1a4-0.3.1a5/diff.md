# Comparing `tmp/neon-skill-stock-0.3.1a4.tar.gz` & `tmp/neon-skill-stock-0.3.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-stock-0.3.1a4.tar", last modified: Fri Jun 23 22:08:43 2023, max compression
+gzip compressed data, was "neon-skill-stock-0.3.1a5.tar", last modified: Fri Jun 23 22:17:38 2023, max compression
```

## Comparing `neon-skill-stock-0.3.1a4.tar` & `neon-skill-stock-0.3.1a5.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.929686 neon-skill-stock-0.3.1a4/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11558 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-23 22:08:43.929686 neon-skill-stock-0.3.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.917686 neon-skill-stock-0.3.1a4/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.913686 neon-skill-stock-0.3.1a4/locale/ca-es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.921686 neon-skill-stock-0.3.1a4/locale/ca-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/ca-es/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/ca-es/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/ca-es/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.921686 neon-skill-stock-0.3.1a4/locale/ca-es/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/ca-es/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.917686 neon-skill-stock-0.3.1a4/locale/de-de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.921686 neon-skill-stock-0.3.1a4/locale/de-de/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/de-de/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/de-de/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/de-de/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.921686 neon-skill-stock-0.3.1a4/locale/de-de/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/de-de/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.917686 neon-skill-stock-0.3.1a4/locale/el-gr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.921686 neon-skill-stock-0.3.1a4/locale/el-gr/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/el-gr/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/el-gr/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.921686 neon-skill-stock-0.3.1a4/locale/el-gr/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/el-gr/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.917686 neon-skill-stock-0.3.1a4/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.921686 neon-skill-stock-0.3.1a4/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/en-us/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/en-us/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/en-us/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.921686 neon-skill-stock-0.3.1a4/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/en-us/intent/stock_price.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.917686 neon-skill-stock-0.3.1a4/locale/es-es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.921686 neon-skill-stock-0.3.1a4/locale/es-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/es-es/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/es-es/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/es-es/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.921686 neon-skill-stock-0.3.1a4/locale/es-es/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/es-es/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.917686 neon-skill-stock-0.3.1a4/locale/fr-fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.921686 neon-skill-stock-0.3.1a4/locale/fr-fr/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/fr-fr/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/fr-fr/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/fr-fr/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.921686 neon-skill-stock-0.3.1a4/locale/fr-fr/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/fr-fr/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.917686 neon-skill-stock-0.3.1a4/locale/gl-es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.925686 neon-skill-stock-0.3.1a4/locale/gl-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/gl-es/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/gl-es/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/gl-es/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.925686 neon-skill-stock-0.3.1a4/locale/gl-es/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/gl-es/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.917686 neon-skill-stock-0.3.1a4/locale/hu-hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.925686 neon-skill-stock-0.3.1a4/locale/hu-hu/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/hu-hu/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/hu-hu/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.925686 neon-skill-stock-0.3.1a4/locale/hu-hu/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/hu-hu/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.917686 neon-skill-stock-0.3.1a4/locale/it-it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.925686 neon-skill-stock-0.3.1a4/locale/it-it/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/it-it/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/it-it/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/it-it/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.925686 neon-skill-stock-0.3.1a4/locale/it-it/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/it-it/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.917686 neon-skill-stock-0.3.1a4/locale/nl-nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.925686 neon-skill-stock-0.3.1a4/locale/nl-nl/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/nl-nl/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/nl-nl/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/nl-nl/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.925686 neon-skill-stock-0.3.1a4/locale/nl-nl/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/nl-nl/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.917686 neon-skill-stock-0.3.1a4/locale/pt-br/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.925686 neon-skill-stock-0.3.1a4/locale/pt-br/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/pt-br/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/pt-br/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/pt-br/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.925686 neon-skill-stock-0.3.1a4/locale/pt-br/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/pt-br/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.917686 neon-skill-stock-0.3.1a4/locale/ru-ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.925686 neon-skill-stock-0.3.1a4/locale/ru-ru/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/ru-ru/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/ru-ru/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.925686 neon-skill-stock-0.3.1a4/locale/ru-ru/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/ru-ru/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.917686 neon-skill-stock-0.3.1a4/locale/sv-se/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.925686 neon-skill-stock-0.3.1a4/locale/sv-se/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/sv-se/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/sv-se/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/sv-se/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.925686 neon-skill-stock-0.3.1a4/locale/sv-se/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/locale/sv-se/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.929686 neon-skill-stock-0.3.1a4/neon_skill_stock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-23 22:08:43.000000 neon-skill-stock-0.3.1a4/neon_skill_stock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-23 22:08:43.000000 neon-skill-stock-0.3.1a4/neon_skill_stock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:08:43.000000 neon-skill-stock-0.3.1a4/neon_skill_stock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 22:08:43.000000 neon-skill-stock-0.3.1a4/neon_skill_stock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 22:08:43.000000 neon-skill-stock-0.3.1a4/neon_skill_stock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 22:08:43.000000 neon-skill-stock-0.3.1a4/neon_skill_stock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 22:08:43.929686 neon-skill-stock-0.3.1a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.929686 neon-skill-stock-0.3.1a4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:08:43.929686 neon-skill-stock-0.3.1a4/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/ui/Stock.qml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/ui/qmldir
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-23 22:08:39.000000 neon-skill-stock-0.3.1a4/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.080883 neon-skill-stock-0.3.1a5/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11558 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-23 22:17:38.080883 neon-skill-stock-0.3.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.068884 neon-skill-stock-0.3.1a5/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.064884 neon-skill-stock-0.3.1a5/locale/ca-es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.068884 neon-skill-stock-0.3.1a5/locale/ca-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/ca-es/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/ca-es/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/ca-es/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.072883 neon-skill-stock-0.3.1a5/locale/ca-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/ca-es/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.064884 neon-skill-stock-0.3.1a5/locale/de-de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.072883 neon-skill-stock-0.3.1a5/locale/de-de/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/de-de/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/de-de/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/de-de/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.072883 neon-skill-stock-0.3.1a5/locale/de-de/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/de-de/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.064884 neon-skill-stock-0.3.1a5/locale/el-gr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.072883 neon-skill-stock-0.3.1a5/locale/el-gr/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/el-gr/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/el-gr/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.072883 neon-skill-stock-0.3.1a5/locale/el-gr/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/el-gr/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.064884 neon-skill-stock-0.3.1a5/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.072883 neon-skill-stock-0.3.1a5/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/en-us/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/en-us/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/en-us/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.072883 neon-skill-stock-0.3.1a5/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/en-us/intent/stock_price.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.064884 neon-skill-stock-0.3.1a5/locale/es-es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.072883 neon-skill-stock-0.3.1a5/locale/es-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/es-es/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/es-es/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/es-es/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.072883 neon-skill-stock-0.3.1a5/locale/es-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/es-es/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.064884 neon-skill-stock-0.3.1a5/locale/fr-fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.072883 neon-skill-stock-0.3.1a5/locale/fr-fr/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/fr-fr/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/fr-fr/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/fr-fr/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.072883 neon-skill-stock-0.3.1a5/locale/fr-fr/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/fr-fr/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.068884 neon-skill-stock-0.3.1a5/locale/gl-es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.076883 neon-skill-stock-0.3.1a5/locale/gl-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/gl-es/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/gl-es/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/gl-es/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.076883 neon-skill-stock-0.3.1a5/locale/gl-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/gl-es/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.068884 neon-skill-stock-0.3.1a5/locale/hu-hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.076883 neon-skill-stock-0.3.1a5/locale/hu-hu/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/hu-hu/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/hu-hu/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.076883 neon-skill-stock-0.3.1a5/locale/hu-hu/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/hu-hu/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.068884 neon-skill-stock-0.3.1a5/locale/it-it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.076883 neon-skill-stock-0.3.1a5/locale/it-it/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/it-it/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/it-it/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/it-it/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.076883 neon-skill-stock-0.3.1a5/locale/it-it/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/it-it/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.068884 neon-skill-stock-0.3.1a5/locale/nl-nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.076883 neon-skill-stock-0.3.1a5/locale/nl-nl/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/nl-nl/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/nl-nl/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/nl-nl/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.076883 neon-skill-stock-0.3.1a5/locale/nl-nl/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/nl-nl/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.068884 neon-skill-stock-0.3.1a5/locale/pt-br/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.076883 neon-skill-stock-0.3.1a5/locale/pt-br/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/pt-br/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/pt-br/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/pt-br/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.076883 neon-skill-stock-0.3.1a5/locale/pt-br/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/pt-br/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.068884 neon-skill-stock-0.3.1a5/locale/ru-ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.076883 neon-skill-stock-0.3.1a5/locale/ru-ru/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/ru-ru/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/ru-ru/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.076883 neon-skill-stock-0.3.1a5/locale/ru-ru/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/ru-ru/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.068884 neon-skill-stock-0.3.1a5/locale/sv-se/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.076883 neon-skill-stock-0.3.1a5/locale/sv-se/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/sv-se/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/sv-se/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/sv-se/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.076883 neon-skill-stock-0.3.1a5/locale/sv-se/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/locale/sv-se/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.080883 neon-skill-stock-0.3.1a5/neon_skill_stock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-23 22:17:38.000000 neon-skill-stock-0.3.1a5/neon_skill_stock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-23 22:17:38.000000 neon-skill-stock-0.3.1a5/neon_skill_stock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:17:38.000000 neon-skill-stock-0.3.1a5/neon_skill_stock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 22:17:38.000000 neon-skill-stock-0.3.1a5/neon_skill_stock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 22:17:38.000000 neon-skill-stock-0.3.1a5/neon_skill_stock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 22:17:38.000000 neon-skill-stock-0.3.1a5/neon_skill_stock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 22:17:38.080883 neon-skill-stock-0.3.1a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.080883 neon-skill-stock-0.3.1a5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:17:38.080883 neon-skill-stock-0.3.1a5/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/ui/Stock.qml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/ui/qmldir
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-23 22:17:33.000000 neon-skill-stock-0.3.1a5/version.py
```

### Comparing `neon-skill-stock-0.3.1a4/LICENSE` & `neon-skill-stock-0.3.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-0.3.1a4/LICENSE.md` & `neon-skill-stock-0.3.1a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-0.3.1a4/PKG-INFO` & `neon-skill-stock-0.3.1a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-stock
-Version: 0.3.1a4
+Version: 0.3.1a5
 Home-page: https://github.com/NeonGeckoCom/skill-stock
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-stock-0.3.1a4/README.md` & `neon-skill-stock-0.3.1a5/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-0.3.1a4/__init__.py` & `neon-skill-stock-0.3.1a5/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-0.3.1a4/neon_skill_stock.egg-info/PKG-INFO` & `neon-skill-stock-0.3.1a5/neon_skill_stock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-stock
-Version: 0.3.1a4
+Version: 0.3.1a5
 Home-page: https://github.com/NeonGeckoCom/skill-stock
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-stock-0.3.1a4/neon_skill_stock.egg-info/SOURCES.txt` & `neon-skill-stock-0.3.1a5/neon_skill_stock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-0.3.1a4/setup.py` & `neon-skill-stock-0.3.1a5/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-0.3.1a4/skill.json` & `neon-skill-stock-0.3.1a5/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-0.3.1a4/test/test_skill.py` & `neon-skill-stock-0.3.1a5/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-0.3.1a4/ui/Stock.qml` & `neon-skill-stock-0.3.1a5/ui/Stock.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-0.3.1a4/version.py` & `neon-skill-stock-0.3.1a5/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.3.1a4"
+__version__ = "0.3.1a5"
```

