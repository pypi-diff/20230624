# Comparing `tmp/neon-skill-fallback_unknown-0.2.3a1.tar.gz` & `tmp/neon-skill-fallback_unknown-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-fallback_unknown-0.2.3a1.tar", last modified: Thu Jun 15 20:52:54 2023, max compression
+gzip compressed data, was "neon-skill-fallback_unknown-1.0.0.tar", last modified: Sat Jun 24 02:13:35 2023, max compression
```

## Comparing `neon-skill-fallback_unknown-0.2.3a1.tar` & `neon-skill-fallback_unknown-1.0.0.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.187169 neon-skill-fallback_unknown-0.2.3a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-15 20:52:54.187169 neon-skill-fallback_unknown-0.2.3a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.175169 neon-skill-fallback_unknown-0.2.3a1/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.175169 neon-skill-fallback_unknown-0.2.3a1/dialog/ca-es/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/ca-es/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/ca-es/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/ca-es/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/ca-es/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.175169 neon-skill-fallback_unknown-0.2.3a1/dialog/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/cs-cz/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/cs-cz/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/cs-cz/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/cs-cz/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.175169 neon-skill-fallback_unknown-0.2.3a1/dialog/da-dk/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/da-dk/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/da-dk/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/da-dk/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/da-dk/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.175169 neon-skill-fallback_unknown-0.2.3a1/dialog/de-de/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/de-de/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/de-de/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/de-de/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/de-de/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.179169 neon-skill-fallback_unknown-0.2.3a1/dialog/en-us/
--rwxr-xr-x   0 runner    (1001) docker     (123)      169 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/en-us/question.dialog
--rwxr-xr-x   0 runner    (1001) docker     (123)      299 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/en-us/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/en-us/websearch.dialog
--rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/en-us/who.is.dialog
--rwxr-xr-x   0 runner    (1001) docker     (123)      134 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/en-us/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.179169 neon-skill-fallback_unknown-0.2.3a1/dialog/es-es/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/es-es/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/es-es/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/es-es/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/es-es/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.179169 neon-skill-fallback_unknown-0.2.3a1/dialog/es-lm/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/es-lm/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/es-lm/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/es-lm/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/es-lm/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.179169 neon-skill-fallback_unknown-0.2.3a1/dialog/eu-eu/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/eu-eu/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/eu-eu/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/eu-eu/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/eu-eu/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.179169 neon-skill-fallback_unknown-0.2.3a1/dialog/fa-fa/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/fa-fa/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/fa-fa/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/fa-fa/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/fa-fa/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.179169 neon-skill-fallback_unknown-0.2.3a1/dialog/fa-ir/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/fa-ir/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/fa-ir/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/fa-ir/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/fa-ir/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.179169 neon-skill-fallback_unknown-0.2.3a1/dialog/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/fr-fr/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/fr-fr/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/fr-fr/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/fr-fr/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.179169 neon-skill-fallback_unknown-0.2.3a1/dialog/gl-es/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/gl-es/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/gl-es/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/gl-es/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/gl-es/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.179169 neon-skill-fallback_unknown-0.2.3a1/dialog/hu-hu/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/hu-hu/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/hu-hu/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/hu-hu/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/hu-hu/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.179169 neon-skill-fallback_unknown-0.2.3a1/dialog/it-it/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/it-it/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/it-it/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/it-it/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/it-it/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.179169 neon-skill-fallback_unknown-0.2.3a1/dialog/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/nl-nl/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/nl-nl/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/nl-nl/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/nl-nl/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.179169 neon-skill-fallback_unknown-0.2.3a1/dialog/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/pl-pl/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/pl-pl/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/pl-pl/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/pl-pl/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.183169 neon-skill-fallback_unknown-0.2.3a1/dialog/pt-br/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/pt-br/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/pt-br/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/pt-br/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/pt-br/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.183169 neon-skill-fallback_unknown-0.2.3a1/dialog/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/ro-ro/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/ro-ro/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/ro-ro/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/ro-ro/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.183169 neon-skill-fallback_unknown-0.2.3a1/dialog/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/ru-ru/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/ru-ru/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/ru-ru/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/ru-ru/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.183169 neon-skill-fallback_unknown-0.2.3a1/dialog/sv-se/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/sv-se/question.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/sv-se/unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/sv-se/who.is.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/dialog/sv-se/why.is.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.183169 neon-skill-fallback_unknown-0.2.3a1/neon_skill_fallback_unknown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-15 20:52:54.000000 neon-skill-fallback_unknown-0.2.3a1/neon_skill_fallback_unknown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-06-15 20:52:54.000000 neon-skill-fallback_unknown-0.2.3a1/neon_skill_fallback_unknown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:52:54.000000 neon-skill-fallback_unknown-0.2.3a1/neon_skill_fallback_unknown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-15 20:52:54.000000 neon-skill-fallback_unknown-0.2.3a1/neon_skill_fallback_unknown.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 20:52:54.000000 neon-skill-fallback_unknown-0.2.3a1/neon_skill_fallback_unknown.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 20:52:54.000000 neon-skill-fallback_unknown-0.2.3a1/neon_skill_fallback_unknown.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:52:54.187169 neon-skill-fallback_unknown-0.2.3a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.183169 neon-skill-fallback_unknown-0.2.3a1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.183169 neon-skill-fallback_unknown-0.2.3a1/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/ui/UnknownIntent.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.175169 neon-skill-fallback_unknown-0.2.3a1/vocab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.183169 neon-skill-fallback_unknown-0.2.3a1/vocab/ca-es/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/ca-es/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/ca-es/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/ca-es/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.183169 neon-skill-fallback_unknown-0.2.3a1/vocab/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/cs-cz/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/cs-cz/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/cs-cz/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.183169 neon-skill-fallback_unknown-0.2.3a1/vocab/da-dk/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/da-dk/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/da-dk/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/da-dk/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.183169 neon-skill-fallback_unknown-0.2.3a1/vocab/de-de/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/de-de/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/de-de/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/de-de/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.183169 neon-skill-fallback_unknown-0.2.3a1/vocab/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/en-us/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/en-us/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/en-us/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.183169 neon-skill-fallback_unknown-0.2.3a1/vocab/es-es/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/es-es/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/es-es/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/es-es/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.183169 neon-skill-fallback_unknown-0.2.3a1/vocab/es-lm/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/es-lm/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/es-lm/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/es-lm/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.183169 neon-skill-fallback_unknown-0.2.3a1/vocab/eu-eu/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/eu-eu/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/eu-eu/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/eu-eu/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.183169 neon-skill-fallback_unknown-0.2.3a1/vocab/fa-fa/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/fa-fa/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/fa-fa/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/fa-fa/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.187169 neon-skill-fallback_unknown-0.2.3a1/vocab/fa-ir/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/fa-ir/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/fa-ir/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/fa-ir/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.187169 neon-skill-fallback_unknown-0.2.3a1/vocab/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/fr-fr/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/fr-fr/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/fr-fr/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.187169 neon-skill-fallback_unknown-0.2.3a1/vocab/gl-es/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/gl-es/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/gl-es/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/gl-es/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.187169 neon-skill-fallback_unknown-0.2.3a1/vocab/hu-hu/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/hu-hu/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/hu-hu/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/hu-hu/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.187169 neon-skill-fallback_unknown-0.2.3a1/vocab/it-it/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/it-it/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/it-it/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/it-it/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.187169 neon-skill-fallback_unknown-0.2.3a1/vocab/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/nl-nl/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/nl-nl/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/nl-nl/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.187169 neon-skill-fallback_unknown-0.2.3a1/vocab/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/pl-pl/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/pl-pl/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/pl-pl/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.187169 neon-skill-fallback_unknown-0.2.3a1/vocab/pt-br/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/pt-br/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/pt-br/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/pt-br/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.187169 neon-skill-fallback_unknown-0.2.3a1/vocab/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/ro-ro/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/ro-ro/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/ro-ro/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.187169 neon-skill-fallback_unknown-0.2.3a1/vocab/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/ru-ru/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/ru-ru/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/ru-ru/why.is.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:54.187169 neon-skill-fallback_unknown-0.2.3a1/vocab/sv-se/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/sv-se/question.voc
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/sv-se/who.is.voc
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 20:52:50.000000 neon-skill-fallback_unknown-0.2.3a1/vocab/sv-se/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.498918 neon-skill-fallback_unknown-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-24 02:13:35.498918 neon-skill-fallback_unknown-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.482918 neon-skill-fallback_unknown-1.0.0/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.486918 neon-skill-fallback_unknown-1.0.0/dialog/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/ca-es/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/ca-es/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/ca-es/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/ca-es/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.486918 neon-skill-fallback_unknown-1.0.0/dialog/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/cs-cz/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/cs-cz/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/cs-cz/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/cs-cz/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.486918 neon-skill-fallback_unknown-1.0.0/dialog/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/da-dk/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/da-dk/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/da-dk/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/da-dk/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.486918 neon-skill-fallback_unknown-1.0.0/dialog/de-de/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/de-de/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/de-de/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/de-de/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/de-de/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.486918 neon-skill-fallback_unknown-1.0.0/dialog/en-us/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      169 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/en-us/question.dialog
+-rwxr-xr-x   0 runner    (1001) docker     (123)      299 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/en-us/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/en-us/websearch.dialog
+-rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/en-us/who.is.dialog
+-rwxr-xr-x   0 runner    (1001) docker     (123)      134 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/en-us/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.486918 neon-skill-fallback_unknown-1.0.0/dialog/es-es/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/es-es/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/es-es/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/es-es/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/es-es/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.486918 neon-skill-fallback_unknown-1.0.0/dialog/es-lm/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/es-lm/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/es-lm/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/es-lm/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/es-lm/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.486918 neon-skill-fallback_unknown-1.0.0/dialog/eu-eu/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/eu-eu/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/eu-eu/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/eu-eu/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/eu-eu/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.486918 neon-skill-fallback_unknown-1.0.0/dialog/fa-fa/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/fa-fa/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/fa-fa/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/fa-fa/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/fa-fa/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.486918 neon-skill-fallback_unknown-1.0.0/dialog/fa-ir/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/fa-ir/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/fa-ir/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/fa-ir/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/fa-ir/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.490918 neon-skill-fallback_unknown-1.0.0/dialog/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/fr-fr/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/fr-fr/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/fr-fr/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/fr-fr/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.490918 neon-skill-fallback_unknown-1.0.0/dialog/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/gl-es/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/gl-es/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/gl-es/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/gl-es/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.490918 neon-skill-fallback_unknown-1.0.0/dialog/hu-hu/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/hu-hu/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/hu-hu/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/hu-hu/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/hu-hu/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.490918 neon-skill-fallback_unknown-1.0.0/dialog/it-it/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/it-it/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/it-it/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/it-it/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/it-it/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.490918 neon-skill-fallback_unknown-1.0.0/dialog/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/nl-nl/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/nl-nl/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/nl-nl/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/nl-nl/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.490918 neon-skill-fallback_unknown-1.0.0/dialog/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/pl-pl/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/pl-pl/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/pl-pl/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/pl-pl/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.490918 neon-skill-fallback_unknown-1.0.0/dialog/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/pt-br/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/pt-br/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/pt-br/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/pt-br/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.490918 neon-skill-fallback_unknown-1.0.0/dialog/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/ro-ro/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/ro-ro/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/ro-ro/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/ro-ro/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.490918 neon-skill-fallback_unknown-1.0.0/dialog/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/ru-ru/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/ru-ru/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/ru-ru/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/ru-ru/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.490918 neon-skill-fallback_unknown-1.0.0/dialog/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/sv-se/question.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/sv-se/unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/sv-se/who.is.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/dialog/sv-se/why.is.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.490918 neon-skill-fallback_unknown-1.0.0/neon_skill_fallback_unknown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-24 02:13:35.000000 neon-skill-fallback_unknown-1.0.0/neon_skill_fallback_unknown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-06-24 02:13:35.000000 neon-skill-fallback_unknown-1.0.0/neon_skill_fallback_unknown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 02:13:35.000000 neon-skill-fallback_unknown-1.0.0/neon_skill_fallback_unknown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-24 02:13:35.000000 neon-skill-fallback_unknown-1.0.0/neon_skill_fallback_unknown.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-24 02:13:35.000000 neon-skill-fallback_unknown-1.0.0/neon_skill_fallback_unknown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-24 02:13:35.000000 neon-skill-fallback_unknown-1.0.0/neon_skill_fallback_unknown.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 02:13:35.498918 neon-skill-fallback_unknown-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/ui/UnknownIntent.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.482918 neon-skill-fallback_unknown-1.0.0/vocab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/vocab/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/ca-es/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/ca-es/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/ca-es/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/vocab/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/cs-cz/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/cs-cz/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/cs-cz/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/vocab/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/da-dk/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/da-dk/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/da-dk/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/vocab/de-de/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/de-de/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/de-de/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/de-de/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/vocab/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/en-us/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/en-us/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/en-us/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/vocab/es-es/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/es-es/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/es-es/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/es-es/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/vocab/es-lm/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/es-lm/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/es-lm/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/es-lm/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/vocab/eu-eu/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/eu-eu/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/eu-eu/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/eu-eu/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/vocab/fa-fa/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/fa-fa/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/fa-fa/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/fa-fa/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/vocab/fa-ir/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/fa-ir/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/fa-ir/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/fa-ir/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/vocab/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/fr-fr/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/fr-fr/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/fr-fr/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/vocab/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/gl-es/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/gl-es/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/gl-es/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/vocab/hu-hu/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/hu-hu/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/hu-hu/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/hu-hu/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/vocab/it-it/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/it-it/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/it-it/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/it-it/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.494918 neon-skill-fallback_unknown-1.0.0/vocab/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/nl-nl/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/nl-nl/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/nl-nl/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.498918 neon-skill-fallback_unknown-1.0.0/vocab/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/pl-pl/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/pl-pl/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/pl-pl/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.498918 neon-skill-fallback_unknown-1.0.0/vocab/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/pt-br/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/pt-br/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/pt-br/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.498918 neon-skill-fallback_unknown-1.0.0/vocab/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/ro-ro/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/ro-ro/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/ro-ro/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.498918 neon-skill-fallback_unknown-1.0.0/vocab/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/ru-ru/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/ru-ru/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/ru-ru/why.is.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:13:35.498918 neon-skill-fallback_unknown-1.0.0/vocab/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/sv-se/question.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/sv-se/who.is.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-24 02:13:32.000000 neon-skill-fallback_unknown-1.0.0/vocab/sv-se/why.is.voc
```

### Comparing `neon-skill-fallback_unknown-0.2.3a1/LICENSE` & `neon-skill-fallback_unknown-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-0.2.3a1/LICENSE.md` & `neon-skill-fallback_unknown-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-0.2.3a1/PKG-INFO` & `neon-skill-fallback_unknown-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-fallback_unknown
-Version: 0.2.3a1
+Version: 1.0.0
 Summary: Neon Unknown Fallback Skill
 Home-page: https://github.com/NeonGeckoCom/skill-fallback_unknown
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `neon-skill-fallback_unknown-0.2.3a1/README.md` & `neon-skill-fallback_unknown-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-0.2.3a1/__init__.py` & `neon-skill-fallback_unknown-1.0.0/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-0.2.3a1/neon_skill_fallback_unknown.egg-info/PKG-INFO` & `neon-skill-fallback_unknown-1.0.0/neon_skill_fallback_unknown.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-fallback-unknown
-Version: 0.2.3a1
+Version: 1.0.0
 Summary: Neon Unknown Fallback Skill
 Home-page: https://github.com/NeonGeckoCom/skill-fallback_unknown
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `neon-skill-fallback_unknown-0.2.3a1/neon_skill_fallback_unknown.egg-info/SOURCES.txt` & `neon-skill-fallback_unknown-1.0.0/neon_skill_fallback_unknown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-0.2.3a1/setup.py` & `neon-skill-fallback_unknown-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-0.2.3a1/skill.json` & `neon-skill-fallback_unknown-1.0.0/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-0.2.3a1/test/test_skill.py` & `neon-skill-fallback_unknown-1.0.0/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-0.2.3a1/ui/UnknownIntent.qml` & `neon-skill-fallback_unknown-1.0.0/ui/UnknownIntent.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_unknown-0.2.3a1/version.py` & `neon-skill-fallback_unknown-1.0.0/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.2.3a1"
+__version__ = "1.0.0"
```

