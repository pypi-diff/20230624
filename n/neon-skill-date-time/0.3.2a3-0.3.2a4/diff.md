# Comparing `tmp/neon-skill-date_time-0.3.2a3.tar.gz` & `tmp/neon-skill-date_time-0.3.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-date_time-0.3.2a3.tar", last modified: Fri Jun 16 21:57:06 2023, max compression
+gzip compressed data, was "neon-skill-date_time-0.3.2a4.tar", last modified: Fri Jun 23 23:24:28 2023, max compression
```

## Comparing `neon-skill-date_time-0.3.2a3.tar` & `neon-skill-date_time-0.3.2a4.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.188549 neon-skill-date_time-0.3.2a3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-16 21:57:06.188549 neon-skill-date_time-0.3.2a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    24069 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.160549 neon-skill-date_time-0.3.2a3/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.160549 neon-skill-date_time-0.3.2a3/locale/ca-es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.160549 neon-skill-date_time-0.3.2a3/locale/ca-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ca-es/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ca-es/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ca-es/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.160549 neon-skill-date_time-0.3.2a3/locale/ca-es/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ca-es/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ca-es/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.164549 neon-skill-date_time-0.3.2a3/locale/ca-es/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ca-es/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ca-es/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ca-es/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ca-es/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.164549 neon-skill-date_time-0.3.2a3/locale/da-dk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.164549 neon-skill-date_time-0.3.2a3/locale/da-dk/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/da-dk/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/da-dk/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/da-dk/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.164549 neon-skill-date_time-0.3.2a3/locale/da-dk/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/da-dk/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/da-dk/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.164549 neon-skill-date_time-0.3.2a3/locale/da-dk/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/da-dk/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/da-dk/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/da-dk/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/da-dk/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.164549 neon-skill-date_time-0.3.2a3/locale/de-de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.164549 neon-skill-date_time-0.3.2a3/locale/de-de/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/de-de/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/de-de/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/de-de/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.164549 neon-skill-date_time-0.3.2a3/locale/de-de/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/de-de/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/de-de/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.164549 neon-skill-date_time-0.3.2a3/locale/de-de/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/de-de/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/de-de/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/de-de/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.164549 neon-skill-date_time-0.3.2a3/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.168549 neon-skill-date_time-0.3.2a3/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/en-us/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/en-us/dialog/date_time_in_location.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/en-us/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/en-us/dialog/time.tz.not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/en-us/dialog/word_friday.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/en-us/dialog/word_monday.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/en-us/dialog/word_saturday.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/en-us/dialog/word_sunday.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/en-us/dialog/word_thursday.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/en-us/dialog/word_tuesday.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/en-us/dialog/word_wednesday.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.168549 neon-skill-date_time-0.3.2a3/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/en-us/intent/what.day.is.it.intent
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/en-us/intent/what.dow.is.it.intent
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/en-us/intent/what.time.is.it.intent
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/en-us/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.168549 neon-skill-date_time-0.3.2a3/locale/es-es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.168549 neon-skill-date_time-0.3.2a3/locale/es-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/es-es/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/es-es/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/es-es/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.168549 neon-skill-date_time-0.3.2a3/locale/es-es/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/es-es/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/es-es/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.168549 neon-skill-date_time-0.3.2a3/locale/es-es/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/es-es/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/es-es/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/es-es/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/es-es/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.168549 neon-skill-date_time-0.3.2a3/locale/eu-eu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.168549 neon-skill-date_time-0.3.2a3/locale/eu-eu/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/eu-eu/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/eu-eu/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/eu-eu/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.168549 neon-skill-date_time-0.3.2a3/locale/eu-eu/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/eu-eu/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/eu-eu/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.168549 neon-skill-date_time-0.3.2a3/locale/eu-eu/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/eu-eu/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/eu-eu/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/eu-eu/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/eu-eu/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.168549 neon-skill-date_time-0.3.2a3/locale/fa-ir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.172549 neon-skill-date_time-0.3.2a3/locale/fa-ir/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fa-ir/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fa-ir/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fa-ir/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.172549 neon-skill-date_time-0.3.2a3/locale/fa-ir/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fa-ir/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fa-ir/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.172549 neon-skill-date_time-0.3.2a3/locale/fa-ir/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fa-ir/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fa-ir/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fa-ir/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fa-ir/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.172549 neon-skill-date_time-0.3.2a3/locale/fr-fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.172549 neon-skill-date_time-0.3.2a3/locale/fr-fr/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fr-fr/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fr-fr/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fr-fr/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.172549 neon-skill-date_time-0.3.2a3/locale/fr-fr/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fr-fr/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fr-fr/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.172549 neon-skill-date_time-0.3.2a3/locale/fr-fr/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fr-fr/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fr-fr/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fr-fr/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/fr-fr/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.172549 neon-skill-date_time-0.3.2a3/locale/gl-es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.172549 neon-skill-date_time-0.3.2a3/locale/gl-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/gl-es/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/gl-es/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/gl-es/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.172549 neon-skill-date_time-0.3.2a3/locale/gl-es/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/gl-es/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/gl-es/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.172549 neon-skill-date_time-0.3.2a3/locale/gl-es/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/gl-es/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/gl-es/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/gl-es/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/gl-es/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.156549 neon-skill-date_time-0.3.2a3/locale/hu-hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.176549 neon-skill-date_time-0.3.2a3/locale/hu-hu/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/hu-hu/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/hu-hu/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/hu-hu/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.176549 neon-skill-date_time-0.3.2a3/locale/hu-hu/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/hu-hu/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.176549 neon-skill-date_time-0.3.2a3/locale/hu-hu/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/hu-hu/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/hu-hu/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/hu-hu/vocab/Time.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.176549 neon-skill-date_time-0.3.2a3/locale/it-it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.176549 neon-skill-date_time-0.3.2a3/locale/it-it/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/it-it/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/it-it/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/it-it/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.176549 neon-skill-date_time-0.3.2a3/locale/it-it/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/it-it/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/it-it/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.176549 neon-skill-date_time-0.3.2a3/locale/it-it/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/it-it/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/it-it/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/it-it/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/it-it/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.156549 neon-skill-date_time-0.3.2a3/locale/nl-nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.176549 neon-skill-date_time-0.3.2a3/locale/nl-nl/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/nl-nl/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/nl-nl/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/nl-nl/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.176549 neon-skill-date_time-0.3.2a3/locale/nl-nl/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/nl-nl/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.176549 neon-skill-date_time-0.3.2a3/locale/nl-nl/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/nl-nl/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/nl-nl/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/nl-nl/vocab/Time.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.176549 neon-skill-date_time-0.3.2a3/locale/pl-pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.176549 neon-skill-date_time-0.3.2a3/locale/pl-pl/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pl-pl/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pl-pl/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pl-pl/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.176549 neon-skill-date_time-0.3.2a3/locale/pl-pl/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pl-pl/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pl-pl/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.180549 neon-skill-date_time-0.3.2a3/locale/pl-pl/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pl-pl/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pl-pl/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pl-pl/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pl-pl/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.180549 neon-skill-date_time-0.3.2a3/locale/pt-br/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.180549 neon-skill-date_time-0.3.2a3/locale/pt-br/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pt-br/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pt-br/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pt-br/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.180549 neon-skill-date_time-0.3.2a3/locale/pt-br/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pt-br/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pt-br/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.180549 neon-skill-date_time-0.3.2a3/locale/pt-br/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pt-br/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pt-br/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pt-br/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/pt-br/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.160549 neon-skill-date_time-0.3.2a3/locale/ro-ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.180549 neon-skill-date_time-0.3.2a3/locale/ro-ro/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ro-ro/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ro-ro/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ro-ro/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.180549 neon-skill-date_time-0.3.2a3/locale/ro-ro/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ro-ro/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.180549 neon-skill-date_time-0.3.2a3/locale/ro-ro/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ro-ro/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ro-ro/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ro-ro/vocab/Time.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.160549 neon-skill-date_time-0.3.2a3/locale/ru-ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.180549 neon-skill-date_time-0.3.2a3/locale/ru-ru/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ru-ru/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ru-ru/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ru-ru/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.180549 neon-skill-date_time-0.3.2a3/locale/ru-ru/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ru-ru/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.180549 neon-skill-date_time-0.3.2a3/locale/ru-ru/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ru-ru/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ru-ru/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/ru-ru/vocab/Time.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.184549 neon-skill-date_time-0.3.2a3/locale/sv-se/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.184549 neon-skill-date_time-0.3.2a3/locale/sv-se/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/sv-se/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/sv-se/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/sv-se/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.184549 neon-skill-date_time-0.3.2a3/locale/sv-se/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/sv-se/regex/location.rx
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/sv-se/timezone.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.184549 neon-skill-date_time-0.3.2a3/locale/sv-se/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/sv-se/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/sv-se/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/sv-se/vocab/Time.voc
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/sv-se/what.time.is.it.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.160549 neon-skill-date_time-0.3.2a3/locale/tr-tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.184549 neon-skill-date_time-0.3.2a3/locale/tr-tr/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/tr-tr/dialog/date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/tr-tr/dialog/time.current.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/tr-tr/dialog/time.tz.not.found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.184549 neon-skill-date_time-0.3.2a3/locale/tr-tr/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/tr-tr/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.184549 neon-skill-date_time-0.3.2a3/locale/tr-tr/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/tr-tr/vocab/Date.voc
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/tr-tr/vocab/Query.voc
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/locale/tr-tr/vocab/Time.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.184549 neon-skill-date_time-0.3.2a3/neon_skill_date_time.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-16 21:57:06.000000 neon-skill-date_time-0.3.2a3/neon_skill_date_time.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-16 21:57:06.000000 neon-skill-date_time-0.3.2a3/neon_skill_date_time.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 21:57:06.000000 neon-skill-date_time-0.3.2a3/neon_skill_date_time.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 21:57:06.000000 neon-skill-date_time-0.3.2a3/neon_skill_date_time.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-16 21:57:06.000000 neon-skill-date_time-0.3.2a3/neon_skill_date_time.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 21:57:06.000000 neon-skill-date_time-0.3.2a3/neon_skill_date_time.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 21:57:06.188549 neon-skill-date_time-0.3.2a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.184549 neon-skill-date_time-0.3.2a3/test/
--rw-r--r--   0 runner    (1001) docker     (123)    21225 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.188549 neon-skill-date_time-0.3.2a3/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/ui/date.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/ui/date2.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/ui/idle.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:57:06.188549 neon-skill-date_time-0.3.2a3/ui/img/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/ui/img/date-bg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/ui/img/date-top.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1061425 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/ui/img/idle-background.png
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/ui/qmldir
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/ui/time.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-16 21:57:01.000000 neon-skill-date_time-0.3.2a3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.927388 neon-skill-date_time-0.3.2a4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-23 23:24:28.927388 neon-skill-date_time-0.3.2a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    24069 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.907387 neon-skill-date_time-0.3.2a4/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.911387 neon-skill-date_time-0.3.2a4/locale/ca-es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.911387 neon-skill-date_time-0.3.2a4/locale/ca-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ca-es/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ca-es/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ca-es/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.911387 neon-skill-date_time-0.3.2a4/locale/ca-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ca-es/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ca-es/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.911387 neon-skill-date_time-0.3.2a4/locale/ca-es/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ca-es/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ca-es/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ca-es/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ca-es/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.911387 neon-skill-date_time-0.3.2a4/locale/da-dk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.911387 neon-skill-date_time-0.3.2a4/locale/da-dk/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/da-dk/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/da-dk/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/da-dk/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.911387 neon-skill-date_time-0.3.2a4/locale/da-dk/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/da-dk/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/da-dk/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.911387 neon-skill-date_time-0.3.2a4/locale/da-dk/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/da-dk/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/da-dk/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/da-dk/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/da-dk/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.911387 neon-skill-date_time-0.3.2a4/locale/de-de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.911387 neon-skill-date_time-0.3.2a4/locale/de-de/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/de-de/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/de-de/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/de-de/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.911387 neon-skill-date_time-0.3.2a4/locale/de-de/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/de-de/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/de-de/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.911387 neon-skill-date_time-0.3.2a4/locale/de-de/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/de-de/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/de-de/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/de-de/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.911387 neon-skill-date_time-0.3.2a4/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.911387 neon-skill-date_time-0.3.2a4/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/en-us/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/en-us/dialog/date_time_in_location.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/en-us/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/en-us/dialog/time.tz.not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/en-us/dialog/word_friday.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/en-us/dialog/word_monday.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/en-us/dialog/word_saturday.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/en-us/dialog/word_sunday.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/en-us/dialog/word_thursday.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/en-us/dialog/word_tuesday.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/en-us/dialog/word_wednesday.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/en-us/intent/what.day.is.it.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/en-us/intent/what.dow.is.it.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/en-us/intent/what.time.is.it.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/en-us/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/es-es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/es-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/es-es/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/es-es/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/es-es/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/es-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/es-es/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/es-es/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/es-es/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/es-es/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/es-es/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/es-es/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/es-es/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/eu-eu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/eu-eu/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/eu-eu/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/eu-eu/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/eu-eu/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/eu-eu/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/eu-eu/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/eu-eu/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/eu-eu/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/eu-eu/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/eu-eu/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/eu-eu/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/eu-eu/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/fa-ir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/fa-ir/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fa-ir/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fa-ir/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fa-ir/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/fa-ir/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fa-ir/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fa-ir/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/fa-ir/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fa-ir/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fa-ir/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fa-ir/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fa-ir/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/fr-fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/fr-fr/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fr-fr/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fr-fr/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fr-fr/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/fr-fr/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fr-fr/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fr-fr/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/fr-fr/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fr-fr/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fr-fr/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fr-fr/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/fr-fr/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.915387 neon-skill-date_time-0.3.2a4/locale/gl-es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.919387 neon-skill-date_time-0.3.2a4/locale/gl-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/gl-es/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/gl-es/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/gl-es/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.919387 neon-skill-date_time-0.3.2a4/locale/gl-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/gl-es/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/gl-es/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.919387 neon-skill-date_time-0.3.2a4/locale/gl-es/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/gl-es/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/gl-es/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/gl-es/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/gl-es/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.907387 neon-skill-date_time-0.3.2a4/locale/hu-hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.919387 neon-skill-date_time-0.3.2a4/locale/hu-hu/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/hu-hu/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/hu-hu/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/hu-hu/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.919387 neon-skill-date_time-0.3.2a4/locale/hu-hu/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/hu-hu/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.919387 neon-skill-date_time-0.3.2a4/locale/hu-hu/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/hu-hu/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/hu-hu/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/hu-hu/vocab/Time.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.919387 neon-skill-date_time-0.3.2a4/locale/it-it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.919387 neon-skill-date_time-0.3.2a4/locale/it-it/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/it-it/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/it-it/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/it-it/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.919387 neon-skill-date_time-0.3.2a4/locale/it-it/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/it-it/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/it-it/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.919387 neon-skill-date_time-0.3.2a4/locale/it-it/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/it-it/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/it-it/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/it-it/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/it-it/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.907387 neon-skill-date_time-0.3.2a4/locale/nl-nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.919387 neon-skill-date_time-0.3.2a4/locale/nl-nl/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/nl-nl/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/nl-nl/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/nl-nl/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.919387 neon-skill-date_time-0.3.2a4/locale/nl-nl/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/nl-nl/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.919387 neon-skill-date_time-0.3.2a4/locale/nl-nl/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/nl-nl/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/nl-nl/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/nl-nl/vocab/Time.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.919387 neon-skill-date_time-0.3.2a4/locale/pl-pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.919387 neon-skill-date_time-0.3.2a4/locale/pl-pl/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pl-pl/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pl-pl/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pl-pl/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.919387 neon-skill-date_time-0.3.2a4/locale/pl-pl/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pl-pl/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pl-pl/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/pl-pl/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pl-pl/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pl-pl/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pl-pl/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pl-pl/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/pt-br/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/pt-br/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pt-br/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pt-br/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pt-br/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/pt-br/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pt-br/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pt-br/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/pt-br/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pt-br/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pt-br/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pt-br/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/pt-br/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.907387 neon-skill-date_time-0.3.2a4/locale/ro-ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/ro-ro/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ro-ro/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ro-ro/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ro-ro/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/ro-ro/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ro-ro/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/ro-ro/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ro-ro/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ro-ro/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ro-ro/vocab/Time.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.907387 neon-skill-date_time-0.3.2a4/locale/ru-ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/ru-ru/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ru-ru/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ru-ru/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ru-ru/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/ru-ru/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ru-ru/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/ru-ru/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ru-ru/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ru-ru/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/ru-ru/vocab/Time.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/sv-se/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/sv-se/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/sv-se/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/sv-se/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/sv-se/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/sv-se/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/sv-se/regex/location.rx
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/sv-se/timezone.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/sv-se/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/sv-se/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/sv-se/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/sv-se/vocab/Time.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/sv-se/what.time.is.it.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.907387 neon-skill-date_time-0.3.2a4/locale/tr-tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/tr-tr/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/tr-tr/dialog/date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/tr-tr/dialog/time.current.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/tr-tr/dialog/time.tz.not.found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.923388 neon-skill-date_time-0.3.2a4/locale/tr-tr/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/tr-tr/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.927388 neon-skill-date_time-0.3.2a4/locale/tr-tr/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/tr-tr/vocab/Date.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/tr-tr/vocab/Query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/locale/tr-tr/vocab/Time.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.927388 neon-skill-date_time-0.3.2a4/neon_skill_date_time.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-23 23:24:28.000000 neon-skill-date_time-0.3.2a4/neon_skill_date_time.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-23 23:24:28.000000 neon-skill-date_time-0.3.2a4/neon_skill_date_time.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 23:24:28.000000 neon-skill-date_time-0.3.2a4/neon_skill_date_time.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-23 23:24:28.000000 neon-skill-date_time-0.3.2a4/neon_skill_date_time.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-23 23:24:28.000000 neon-skill-date_time-0.3.2a4/neon_skill_date_time.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 23:24:28.000000 neon-skill-date_time-0.3.2a4/neon_skill_date_time.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 23:24:28.927388 neon-skill-date_time-0.3.2a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.927388 neon-skill-date_time-0.3.2a4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    21225 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.927388 neon-skill-date_time-0.3.2a4/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/ui/date.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/ui/date2.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/ui/idle.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:24:28.927388 neon-skill-date_time-0.3.2a4/ui/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/ui/img/date-bg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/ui/img/date-top.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1061425 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/ui/img/idle-background.png
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/ui/qmldir
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/ui/time.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-23 23:24:24.000000 neon-skill-date_time-0.3.2a4/version.py
```

### Comparing `neon-skill-date_time-0.3.2a3/LICENSE` & `neon-skill-date_time-0.3.2a4/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-0.3.2a3/LICENSE.md` & `neon-skill-date_time-0.3.2a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-0.3.2a3/PKG-INFO` & `neon-skill-date_time-0.3.2a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-date_time
-Version: 0.3.2a3
+Version: 0.3.2a4
 Home-page: https://github.com/NeonGeckoCom/skill-date_time
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-date_time-0.3.2a3/README.md` & `neon-skill-date_time-0.3.2a4/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-0.3.2a3/__init__.py` & `neon-skill-date_time-0.3.2a4/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-0.3.2a3/neon_skill_date_time.egg-info/PKG-INFO` & `neon-skill-date_time-0.3.2a4/neon_skill_date_time.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-date-time
-Version: 0.3.2a3
+Version: 0.3.2a4
 Home-page: https://github.com/NeonGeckoCom/skill-date_time
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-date_time-0.3.2a3/neon_skill_date_time.egg-info/SOURCES.txt` & `neon-skill-date_time-0.3.2a4/neon_skill_date_time.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-0.3.2a3/setup.py` & `neon-skill-date_time-0.3.2a4/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-0.3.2a3/skill.json` & `neon-skill-date_time-0.3.2a4/skill.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974747474747474%*

 * *Differences: {"'requirements'": "{'python': {insert: [(2, 'ovos-bus-client~=0.0.4'), (3, 'ovos-utils~=0.0.34'), "*

 * *                   "(4, 'pytz>=2022.1')], delete: [4, 3, 2]}}"}*

```diff
@@ -28,17 +28,17 @@
         "arm64",
         "arm"
     ],
     "requirements": {
         "python": [
             "geocoder~=1.38",
             "neon-utils~=1.3",
-            "ovos-bus-client~=0.0.3",
-            "ovos-utils~=0.0.28",
-            "pytz>=2017.2",
+            "ovos-bus-client~=0.0.4",
+            "ovos-utils~=0.0.34",
+            "pytz>=2022.1",
             "timezonefinder~=5.2"
         ],
         "skill": [],
         "system": {}
     },
     "short_description": "Get the time, date, day of the week",
     "skillname": "skill-date_time",
```

### Comparing `neon-skill-date_time-0.3.2a3/test/test_skill.py` & `neon-skill-date_time-0.3.2a4/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-0.3.2a3/ui/date.qml` & `neon-skill-date_time-0.3.2a4/ui/date.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-0.3.2a3/ui/date2.qml` & `neon-skill-date_time-0.3.2a4/ui/date2.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-0.3.2a3/ui/idle.qml` & `neon-skill-date_time-0.3.2a4/ui/idle.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-0.3.2a3/ui/img/idle-background.png` & `neon-skill-date_time-0.3.2a4/ui/img/idle-background.png`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-0.3.2a3/ui/time.qml` & `neon-skill-date_time-0.3.2a4/ui/time.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-date_time-0.3.2a3/version.py` & `neon-skill-date_time-0.3.2a4/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.3.2a3"
+__version__ = "0.3.2a4"
```

