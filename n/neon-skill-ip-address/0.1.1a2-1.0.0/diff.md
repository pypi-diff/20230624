# Comparing `tmp/neon-skill-ip_address-0.1.1a2.tar.gz` & `tmp/neon-skill-ip_address-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-ip_address-0.1.1a2.tar", last modified: Thu Jun 15 21:01:26 2023, max compression
+gzip compressed data, was "neon-skill-ip_address-1.0.0.tar", last modified: Fri Jun 23 23:42:52 2023, max compression
```

## Comparing `neon-skill-ip_address-0.1.1a2.tar` & `neon-skill-ip_address-1.0.0.tar`

### file list

```diff
@@ -1,93 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:01:26.361148 neon-skill-ip_address-0.1.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-15 21:01:26.361148 neon-skill-ip_address-0.1.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:01:26.349148 neon-skill-ip_address-0.1.1a2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:01:26.349148 neon-skill-ip_address-0.1.1a2/locale/ca-es/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/ca-es/IP.voc
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/ca-es/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/ca-es/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/ca-es/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/ca-es/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/ca-es/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:01:26.349148 neon-skill-ip_address-0.1.1a2/locale/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/cs-cz/IP.voc
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/cs-cz/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/cs-cz/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/cs-cz/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/cs-cz/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/cs-cz/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:01:26.353148 neon-skill-ip_address-0.1.1a2/locale/de-de/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/de-de/IP.voc
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/de-de/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/de-de/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/de-de/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/de-de/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/de-de/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:01:26.353148 neon-skill-ip_address-0.1.1a2/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/en-us/IP.voc
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/en-us/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/en-us/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/en-us/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/en-us/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/en-us/public.voc
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/en-us/query.voc
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/en-us/word_local.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/en-us/word_public.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:01:26.353148 neon-skill-ip_address-0.1.1a2/locale/es-es/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/es-es/IP.voc
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/es-es/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/es-es/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/es-es/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/es-es/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/es-es/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:01:26.353148 neon-skill-ip_address-0.1.1a2/locale/eu-eu/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/eu-eu/IP.voc
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/eu-eu/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/eu-eu/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/eu-eu/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/eu-eu/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/eu-eu/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:01:26.357148 neon-skill-ip_address-0.1.1a2/locale/it-it/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/it-it/IP.voc
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/it-it/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/it-it/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/it-it/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/it-it/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/it-it/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:01:26.357148 neon-skill-ip_address-0.1.1a2/locale/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/pl-pl/IP.voc
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/pl-pl/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/pl-pl/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/pl-pl/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/pl-pl/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/pl-pl/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:01:26.357148 neon-skill-ip_address-0.1.1a2/locale/pt-br/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/pt-br/IP.voc
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/pt-br/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/pt-br/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/pt-br/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/pt-br/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/pt-br/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:01:26.357148 neon-skill-ip_address-0.1.1a2/locale/sv-se/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/sv-se/IP.voc
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/sv-se/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/sv-se/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/sv-se/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/sv-se/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/locale/sv-se/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:01:26.361148 neon-skill-ip_address-0.1.1a2/neon_skill_ip_address.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-15 21:01:26.000000 neon-skill-ip_address-0.1.1a2/neon_skill_ip_address.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-15 21:01:26.000000 neon-skill-ip_address-0.1.1a2/neon_skill_ip_address.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:01:26.000000 neon-skill-ip_address-0.1.1a2/neon_skill_ip_address.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 21:01:26.000000 neon-skill-ip_address-0.1.1a2/neon_skill_ip_address.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 21:01:26.000000 neon-skill-ip_address-0.1.1a2/neon_skill_ip_address.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 21:01:26.000000 neon-skill-ip_address-0.1.1a2/neon_skill_ip_address.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:01:26.361148 neon-skill-ip_address-0.1.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:01:26.361148 neon-skill-ip_address-0.1.1a2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 21:01:21.000000 neon-skill-ip_address-0.1.1a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:52.142220 neon-skill-ip_address-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-23 23:42:52.142220 neon-skill-ip_address-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:52.130220 neon-skill-ip_address-1.0.0/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:52.130220 neon-skill-ip_address-1.0.0/locale/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/ca-es/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/ca-es/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/ca-es/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/ca-es/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/ca-es/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/ca-es/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:52.130220 neon-skill-ip_address-1.0.0/locale/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/cs-cz/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/cs-cz/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/cs-cz/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/cs-cz/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/cs-cz/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/cs-cz/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:52.134220 neon-skill-ip_address-1.0.0/locale/de-de/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/de-de/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/de-de/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/de-de/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/de-de/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/de-de/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/de-de/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:52.134220 neon-skill-ip_address-1.0.0/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/en-us/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/en-us/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/en-us/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/en-us/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/en-us/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/en-us/public.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/en-us/query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/en-us/word_local.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/en-us/word_public.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:52.134220 neon-skill-ip_address-1.0.0/locale/es-es/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/es-es/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/es-es/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/es-es/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/es-es/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/es-es/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/es-es/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:52.134220 neon-skill-ip_address-1.0.0/locale/eu-eu/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/eu-eu/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/eu-eu/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/eu-eu/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/eu-eu/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/eu-eu/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/eu-eu/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:52.138220 neon-skill-ip_address-1.0.0/locale/it-it/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/it-it/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/it-it/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/it-it/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/it-it/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/it-it/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/it-it/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:52.138220 neon-skill-ip_address-1.0.0/locale/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/pl-pl/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/pl-pl/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/pl-pl/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/pl-pl/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/pl-pl/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/pl-pl/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:52.138220 neon-skill-ip_address-1.0.0/locale/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/pt-br/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/pt-br/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/pt-br/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/pt-br/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/pt-br/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/pt-br/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:52.138220 neon-skill-ip_address-1.0.0/locale/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/sv-se/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/sv-se/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/sv-se/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/sv-se/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/sv-se/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/locale/sv-se/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:52.138220 neon-skill-ip_address-1.0.0/neon_skill_ip_address.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-23 23:42:52.000000 neon-skill-ip_address-1.0.0/neon_skill_ip_address.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-23 23:42:52.000000 neon-skill-ip_address-1.0.0/neon_skill_ip_address.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 23:42:52.000000 neon-skill-ip_address-1.0.0/neon_skill_ip_address.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-23 23:42:52.000000 neon-skill-ip_address-1.0.0/neon_skill_ip_address.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-23 23:42:52.000000 neon-skill-ip_address-1.0.0/neon_skill_ip_address.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-23 23:42:52.000000 neon-skill-ip_address-1.0.0/neon_skill_ip_address.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 23:42:52.142220 neon-skill-ip_address-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:52.138220 neon-skill-ip_address-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:52.138220 neon-skill-ip_address-1.0.0/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/ui/qmldir
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-23 23:42:49.000000 neon-skill-ip_address-1.0.0/version.py
```

### Comparing `neon-skill-ip_address-0.1.1a2/LICENSE` & `neon-skill-ip_address-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-0.1.1a2/LICENSE.md` & `neon-skill-ip_address-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-0.1.1a2/PKG-INFO` & `neon-skill-ip_address-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-ip_address
-Version: 0.1.1a2
+Version: 1.0.0
 Summary: Neon IP Address Skill
 Home-page: https://github.com/NeonGeckoCom/skill-ip_address
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `neon-skill-ip_address-0.1.1a2/README.md` & `neon-skill-ip_address-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-0.1.1a2/__init__.py` & `neon-skill-ip_address-1.0.0/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-0.1.1a2/neon_skill_ip_address.egg-info/PKG-INFO` & `neon-skill-ip_address-1.0.0/neon_skill_ip_address.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-ip-address
-Version: 0.1.1a2
+Version: 1.0.0
 Summary: Neon IP Address Skill
 Home-page: https://github.com/NeonGeckoCom/skill-ip_address
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `neon-skill-ip_address-0.1.1a2/neon_skill_ip_address.egg-info/SOURCES.txt` & `neon-skill-ip_address-1.0.0/neon_skill_ip_address.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -70,8 +70,9 @@
 locale/sv-se/query.voc
 neon_skill_ip_address.egg-info/PKG-INFO
 neon_skill_ip_address.egg-info/SOURCES.txt
 neon_skill_ip_address.egg-info/dependency_links.txt
 neon_skill_ip_address.egg-info/entry_points.txt
 neon_skill_ip_address.egg-info/requires.txt
 neon_skill_ip_address.egg-info/top_level.txt
-test/test_skill.py
+test/test_skill.py
+ui/qmldir
```

### Comparing `neon-skill-ip_address-0.1.1a2/setup.py` & `neon-skill-ip_address-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-0.1.1a2/skill.json` & `neon-skill-ip_address-1.0.0/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-0.1.1a2/test/test_skill.py` & `neon-skill-ip_address-1.0.0/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-0.1.1a2/version.py` & `neon-skill-ip_address-1.0.0/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.1.1a2"
+__version__ = "1.0.0"
```

