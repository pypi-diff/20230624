# Comparing `tmp/FuncsForSPO-6.0.2.tar.gz` & `tmp/FuncsForSPO-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-6.0.2.tar", last modified: Tue Jun 20 14:43:28 2023, max compression
+gzip compressed data, was "FuncsForSPO-6.1.0.tar", last modified: Sat Jun 24 21:18:55 2023, max compression
```

## Comparing `FuncsForSPO-6.0.2.tar` & `FuncsForSPO-6.1.0.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.456146 FuncsForSPO-6.0.2/
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.045098 FuncsForSPO-6.0.2/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.105942 FuncsForSPO-6.0.2/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.0.2/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.0.2/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.117531 FuncsForSPO-6.0.2/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.2/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.0.2/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.125530 FuncsForSPO-6.0.2/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.2/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.0.2/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.133376 FuncsForSPO-6.0.2/FuncsForSPO/flanguage/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.0.2/FuncsForSPO/flanguage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.137567 FuncsForSPO-6.0.2/FuncsForSPO/flanguage/translator/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.0.2/FuncsForSPO/flanguage/translator/__init__.py
--rw-rw-rw-   0        0        0      817 2023-06-05 14:56:55.000000 FuncsForSPO-6.0.2/FuncsForSPO/flanguage/translator/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.148383 FuncsForSPO-6.0.2/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.2/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.0.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.155055 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.191304 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0     8203 2023-06-19 21:37:07.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
--rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
--rw-rw-rw-   0        0        0     1340 2023-06-17 20:27:40.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.211433 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.227744 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.234308 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.262342 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/base.py
--rw-rw-rw-   0        0        0     8971 2023-06-18 22:41:54.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.272864 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.314948 FuncsForSPO-6.0.2/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.329481 FuncsForSPO-6.0.2/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    67096 2023-06-03 13:16:56.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.347521 FuncsForSPO-6.0.2/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.2/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-6.0.2/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.359364 FuncsForSPO-6.0.2/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.2/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39083 2023-06-06 21:05:50.000000 FuncsForSPO-6.0.2/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.370694 FuncsForSPO-6.0.2/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.2/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.0.2/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.380329 FuncsForSPO-6.0.2/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.0.2/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.0.2/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.386213 FuncsForSPO-6.0.2/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-6.0.2/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.094337 FuncsForSPO-6.0.2/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8026 2023-06-20 14:43:27.000000 FuncsForSPO-6.0.2/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1886 2023-06-20 14:43:27.000000 FuncsForSPO-6.0.2/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 14:43:27.000000 FuncsForSPO-6.0.2/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-06-20 14:43:27.000000 FuncsForSPO-6.0.2/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      458 2023-06-20 14:43:27.000000 FuncsForSPO-6.0.2/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.0.2/LICENSE
--rw-rw-rw-   0        0        0     8026 2023-06-20 14:43:28.451626 FuncsForSPO-6.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-6.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-20 14:43:28.456146 FuncsForSPO-6.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2611 2023-06-20 14:43:11.000000 FuncsForSPO-6.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.457711 FuncsForSPO-6.1.0/
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.073004 FuncsForSPO-6.1.0/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.134342 FuncsForSPO-6.1.0/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.1.0/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.1.0/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.145359 FuncsForSPO-6.1.0/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.0/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.1.0/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.155949 FuncsForSPO-6.1.0/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.0/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.1.0/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.160476 FuncsForSPO-6.1.0/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.0/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.178476 FuncsForSPO-6.1.0/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.0/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.1.0/FuncsForSPO/flanguage/translator/__translator.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.0/FuncsForSPO/flanguage/translator/base.py
+-rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.1.0/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.190479 FuncsForSPO-6.1.0/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.0/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.1.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.195475 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.230527 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0     8203 2023-06-19 21:37:07.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
+-rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
+-rw-rw-rw-   0        0        0     1340 2023-06-17 20:27:40.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.250535 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.267068 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.274070 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.303074 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/base.py
+-rw-rw-rw-   0        0        0     8971 2023-06-18 22:41:54.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.316130 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.326126 FuncsForSPO-6.1.0/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.337127 FuncsForSPO-6.1.0/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    69692 2023-06-24 21:18:37.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.348133 FuncsForSPO-6.1.0/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.0/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.1.0/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.362687 FuncsForSPO-6.1.0/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.0/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39083 2023-06-06 21:05:50.000000 FuncsForSPO-6.1.0/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.374694 FuncsForSPO-6.1.0/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.0/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.1.0/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.384683 FuncsForSPO-6.1.0/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.1.0/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.1.0/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.390684 FuncsForSPO-6.1.0/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.1.0/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.124353 FuncsForSPO-6.1.0/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8023 2023-06-24 21:18:54.000000 FuncsForSPO-6.1.0/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1976 2023-06-24 21:18:54.000000 FuncsForSPO-6.1.0/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 21:18:54.000000 FuncsForSPO-6.1.0/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-06-24 21:18:54.000000 FuncsForSPO-6.1.0/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      458 2023-06-24 21:18:54.000000 FuncsForSPO-6.1.0/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.1.0/LICENSE
+-rw-rw-rw-   0        0        0     8023 2023-06-24 21:18:55.454168 FuncsForSPO-6.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 21:18:55.457711 FuncsForSPO-6.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2611 2023-06-24 21:16:16.000000 FuncsForSPO-6.1.0/setup.py
```

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/femails/femails.py` & `FuncsForSPO-6.1.0/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/flanguage/translator/translator.py` & `FuncsForSPO-6.1.0/FuncsForSPO/flanguage/translator/translator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 
-def translate_text(text, source_lang='en', target_lang='pt'):
+def translate_text(text, source_lang='auto_awesome', target_lang='pt'):
     """
     Translates the given text from the source language to the target language using MyMemory API.
     
     :param text: The text to be translated.
     :type text: str
     
     :param source_lang: The language code of the source language. Default is 'en' for English.
@@ -15,8 +15,8 @@
     
     :return: The translated text.
     :rtype: str
     """
     url = f"https://api.mymemory.translated.net/get?q={text}&langpair={source_lang}|{target_lang}"
     response = requests.get(url)
     translation = response.json()["responseData"]["translatedText"]
-    return translation
+    return translation
```

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/__ocr_online_v2.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/__ocr_online_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/base.py` & `FuncsForSPO-6.1.0/FuncsForSPO/flanguage/translator/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/pdfutils/pdfutils.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Funções de front-end para PySimpleGUI
 
 """
 
 import os
 import sys
 import PySimpleGUI as sg
-from FuncsForSPO.fpython.functions_for_py import retorna_home_user
+from FuncsForSPO.fpython.functions_for_py import *
 
 ########## For PySimpleGUI ########
 def resource_path(relative_path):
     """ Get absolute path to resource, works for dev and for PyInstaller 
     
         SE QUISER ADICIONAR ALGO NO ROBÔ BASTA USAR ESSA FUNÇÃO PARA ADICIONAR O CAMINHO PARA O EXECUTÁVEL COLOCAR
     """
@@ -83,15 +83,15 @@
     else:
         return sg.popup_get_text(text,
                     title=title,
                     background_color=back_color,
                     password_char=password_char
                     )
 
-def popup_get_folder(title: str='Recuperar Pasta', text: str='Insira o caminho da pasta...', default_path=os.path.join(retorna_home_user(), 'Downloads'), no_window=False, theme: str='Material1', back_color: str='#E0E3E4') -> str|None:
+def popup_get_folder(title: str='Recuperar Pasta', text: str='Insira o caminho da pasta...', default_path=os.path.join(os.path.expanduser("~"), 'Downloads'), no_window=False, theme: str='Material1', back_color: str='#E0E3E4') -> str|None:
     """Popup para buscar pasta (Não arquivo)
 
     Args:
         title (str, optional): Titulo da janela. Defaults to 'Recuperar Pasta'.
         text (str, optional): Texto da janela (if no_window is False). Defaults to 'Insira o caminho da pasta...'.
         default_path (str, optional): Caminho padrão para o usuário visualizar. Defaults to os.path.join(retorna_home_user(), 'Downloads').
         no_window (bool, optional): Não mostrar a janela. Defaults to False.
```

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fpython/functions_for_py.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from fnmatch import fnmatch
 from time import sleep
 import os, sys, shutil, platform, re, logging, unicodedata, gc, requests, time, json, threading
 import subprocess as sp
 import zipfile
 from rich import print
 from numpy import unicode_
+from FuncsForSPO.fgpt.fgpt import *
 ################################## IMPORTS #############################################
 
 def remover_acentos(text:str, encoding:str='utf-8'):
 	try:
 		text = unicode_(text, encoding=encoding)
 	except Exception:
 		pass
@@ -1328,41 +1329,86 @@
             return valor
     valor = f'{valor:_.2f}'
     valor = valor.replace('.', ',').replace('_', '.')
     if sigl:
         return 'R$ '+valor
     return valor
 
-def cria_diretorios_para_novo_projeto_python(create_base_dir:bool=True, packages:str='FuncsForSPO'):
+def cria_diretorios_para_novo_projeto_python(with_draft=False, create_base_dir:bool=True, packages:str='FuncsForSPO'):
     """# ATENÇÃO, UTILIZAR SOMENTE UMA VEZ NO MOMENTO DA CRIAÇÃO DO NOVO PROJETO!
     
     create_base_dir: cria o diretorio para o user colocar a base
     packages: instala pacotes necessários
+    
+    with_draft deve ser como nesse exemplo:
+        # 1. importe from src.base.base import * no app.py
+        # 2. crie um bot com o uso abaixo que entre nesse site: https://www.pythonanywhere.com/login/
+        # 3. envie o usuário que virá no arquivo config.json em BOT USUARIO nesse seletor: #id_auth-username
+        # 4. envie também a senha que virá no arquivo config.json em BOT SENHA nesse seletor: #id_auth-password
+        # 5. e clique em login nesse seletor: #id_next
+        # 6. espere 5 segundos
+        
+        o resultado esperado no arquivo app.py é:
+        
+        >>> from src.base.base import *
+        >>> class RobotClass(Bot):
+        >>>    def __init__(self) -> None:
+        >>>        self.configs = read_json(CONFIG_PATH)
+        >>>        self.HEADLESS = self.configs['BOT']['HEADLESS']
+        >>>        self.DOWNLOAD_FILES = False
+        >>>        super().__init__(self.HEADLESS, self.DOWNLOAD_FILES)
+        >>>        
+        >>>    def run(self):
+        >>>        self.DRIVER.get("https://www.pythonanywhere.com/login/")
+        >>>        username = self.configs['BOT']['USUARIO']
+        >>>        password = self.configs['BOT']['SENHA']
+        >>>        self.WDW10.until(EC.presence_of_element_located((By.ID, 'id_auth-username')))
+        >>>        self.DRIVER.find_element_by_id('id_auth-username').send_keys(username)
+        >>>        self.DRIVER.find_element_by_id('id_auth-password').send_keys(password)
+        >>>        self.DRIVER.find_element_by_id('id_next').click()
+        >>>        time.sleep(5) # Espera 5 segundos antes de encerrar a execução.
     """
     faz_log('Criando pasta e arquivo de logs com esse log...')
     # cria diretório src
     cria_dir_no_dir_de_trabalho_atual('src')
     APP_PATH = arquivo_com_caminho_absoluto(['src', 'app'], 'app.py')
     BASE_PATH = arquivo_com_caminho_absoluto(['src', 'base'], 'base.py')
     DATABASE_PATH = arquivo_com_caminho_absoluto(['src', 'database'], 'database.py')
     EXCEPTIONS_PATH = arquivo_com_caminho_absoluto(['src', 'exceptions'], 'exceptioins.py')
     CONFIG_PATH = arquivo_com_caminho_absoluto(['bin'], 'config.json')
     UTILS_PATH = arquivo_com_caminho_absoluto(['src', 'utils'], 'utils.py')
     TESTS_PATH = arquivo_com_caminho_absoluto(['src', 'tests'], 'tests.py')
     # cria subdiretorios do src
 
-    # CRIA ARQUIVO PYTHON EM SRC\\APP
-    with open(APP_PATH, 'w', encoding='utf-8') as f:
-        f.write("""from src.base.base import *
+    if not isinstance(with_draft, str):
+        # CRIA ARQUIVO PYTHON EM SRC\\APP
+        with open(APP_PATH, 'w', encoding='utf-8') as f:
+            f.write("""from src.base.base import *
+    class RobotClass(Bot):
+        def __init__(self) -> None:
+            self.configs = read_json(CONFIG_PATH)
+            self.HEADLESS = self.configs['BOT']['HEADLESS']
+            self.DOWNLOAD_FILES = False
+            super().__init__(self.HEADLESS, self.DOWNLOAD_FILES)
+    """)
+    else:
+        print('Criando arquivo com draft... É MUITO IMPORTANTE VOCÊ VER SE FICOU BOM COMO O GPT ESCREVEU O CÓDIGO!\nEscreve apenas no arquivo app.py, se precisar colocar dados do usuário no Json, adiicone manualmente')
+        # CRIA ARQUIVO PYTHON EM SRC\\APP
+        from FuncsForSPO.utils.utils import GPT_WITH_DRAFT_PROMPT
+        response_gpt = gpt(GPT_WITH_DRAFT_PROMPT.replace('DRAFT_USER', with_draft))
+        with open(APP_PATH, 'w', encoding='utf-8') as f:
+            f.write(f"""from src.base.base import *
 class RobotClass(Bot):
     def __init__(self) -> None:
         self.configs = read_json(CONFIG_PATH)
-        # self.HEADLESS = self.configs['SCHEMA']['HEADLESS']
-        # self.DOWNLOAD_FILES = self.configs['SCHEMA']['DOWNLOAD_FILES']
-        # super().__init__(self.HEADLESS, self.DOWNLOAD_FILES)
+        self.HEADLESS = self.configs['BOT']['HEADLESS']
+        self.DOWNLOAD_FILES = False
+        super().__init__(self.HEADLESS, self.DOWNLOAD_FILES)
+        
+    {response_gpt}
 """)
 
     # CRIA ARQUIVO PYTHON EM base
     with open(BASE_PATH, 'w', encoding='utf-8') as f:
         f.write("""from selenium.webdriver import Chrome
 from selenium import webdriver
 from selenium.webdriver.common.keys import Keys
@@ -1551,18 +1597,18 @@
     with open(EXCEPTIONS_PATH, 'w', encoding='utf-8') as f:
         f.write("""from FuncsForSPO.fexceptions.exceptions import *
 """)
     
     # cria arquivo json
     with open(CONFIG_PATH, 'w', encoding='utf-8') as fjson:
         fjson.write("""{
-    "CONFIG": {
-        "STRING": "STRING",
-        "INT": 1,
-        "BOOL": true
+    "BOT": {
+        "USER": "USER",
+        "PASSWORD": "PASSWORD",
+        "HEADLESS": true
         }
 }""")
         
     # cria arquivo utils
     with open(UTILS_PATH, 'w', encoding='utf-8') as fjson:
         fjson.write("""""")
```

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fregex/functions_re.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Aqui você encontrará algumas funções utilizando Regex
 
 Se necessário, colaborem =)
 """
 
 ########### imports ##############
 import re
-from FuncsForSPO.fpython.functions_for_py import faz_log, pega_somente_numeros
+from FuncsForSPO.fpython.functions_for_py import *
 ########### imports ##############
 
 def extrair_datas_re_input(text: str, pattern: str) -> str:
     """### Retorna datas no padrão escolhido
 
     Args:
         text (str): texto que tem datas
```

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-6.1.0/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO/utils/utils.py` & `FuncsForSPO-6.1.0/FuncsForSPO/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -996,8 +996,181 @@
 'Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, como Gecko) Chrome/42.0.2311.135 Safari/537.36',
 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_2) AppleWebKit/537.36 (KHTML, como Gecko) Chrome/43.0.2357.130 Safari/537.36',
 'Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, como Gecko) coc_coc_browser/50.0.125 Chrome/44.0.2403.125 Safari/537.36',
 'Mozilla/5.0 (compatível; MSIE 10,0; Windows NT 6.1; WOW64; Tridente/6,0; SLCC2; .NET CLR 2.0.50727; . NET4.0C; . NET4.0E)',
 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_5) AppleWebKit/537.36 (KHTML, como Gecko) Chrome/43.0.2357.124 Safari/537.36',
 'Mozilla/5.0 (Windows NT 6.3; Win64; x64; Tridente/7,0; MAARJS; rv: 11.0) como Gecko',
 'Mozilla/5.0 (Linux; Android 5.0; SAMSUNG SM-N900T Build/LRX21V) AppleWebKit/537.36 (KHTML, como Gecko) SamsungBrowser/2.1 Chrome/34.0.1847.76 Mobile Safari/537.36',
-'Mozilla/5.0 (iPhone; CPU iPhone OS 8_4 como Mac OS X) AppleWebKit/600.1.4 (KHTML, como Gecko) GSA/7.0.55539 Mobile/12H143 Safari/600.1.4']
+'Mozilla/5.0 (iPhone; CPU iPhone OS 8_4 como Mac OS X) AppleWebKit/600.1.4 (KHTML, como Gecko) GSA/7.0.55539 Mobile/12H143 Safari/600.1.4']
+
+
+GPT_WITH_DRAFT_PROMPT="""
+considerando que meu projeto tem esse formato:
+
+|-base
+|---base.xlsx
+|-bin
+|---config.json
+|-logs
+|---logs.log
+|-src
+|---app
+|------app.py
+|---base
+|------base.py
+|---database
+|------database.py
+|---exceptions
+|------exceptions.py
+|---tests
+|------tests.py
+|---utils
+|------utils.py
+|-venv
+main.py
+
+considerando que dentro de app.py contem o seguinte código python considerando:
+
+from src.base.base import *
+
+class RobotClass(Bot):
+    def __init__(self) -> None:
+        self.configs = read_json(CONFIG_PATH)
+        self.HEADLESS = self.configs['BOT']['HEADLESS']
+        self.DOWNLOAD_FILES = True
+        super().__init__(self.HEADLESS, self.DOWNLOAD_FILES)
+
+
+e que Bot herda de base.py que tem esse conteúdo:
+
+from selenium.webdriver import Chrome
+from selenium import webdriver
+from selenium.webdriver.common.keys import Keys
+from selenium.webdriver.chrome.options import Options as ChromeOptions
+from selenium.webdriver.chrome.service import Service
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support.wait import WebDriverWait
+from selenium.common.exceptions import *
+from webdriver_manager.chrome import ChromeDriverManager
+from FuncsForSPO.fpython.functions_for_py import *
+from FuncsForSPO.fselenium.functions_selenium import *
+from FuncsForSPO.fwinotify.fwinotify import *
+from FuncsForSPO.fregex.functions_re import *
+import pandas as pd
+import json
+import os
+
+# -- GLOBAL -- #
+URL_SUPORTE = f'https://api.whatsapp.com/send?phone=5511985640273'
+CONFIG_PATH = arquivo_com_caminho_absoluto('bin', 'config.json')
+BASE = os.path.abspath('base')
+DOWNLOAD_DIR =  cria_dir_no_dir_de_trabalho_atual(dir='downloads', print_value=False, criar_diretorio=True)
+limpa_diretorio(DOWNLOAD_DIR)
+# -- GLOBAL -- #
+
+class Bot:    
+    def __init__(self, headless, download_files) -> None:
+        # --- CHROME OPTIONS --- #
+        self._options = ChromeOptions()
+        
+        if download_files:
+            # --- PATH BASE DIR --- #
+            self._SETTINGS_SAVE_AS_PDF = {
+                        "recentDestinations": [
+                            {
+                                "id": "Save as PDF",
+                                "origin": "local",
+                                "account": ""
+                            }
+                        ],
+                        "selectedDestinationId": "Save as PDF",
+                        "version": 2,
+                    }
+
+
+            self._PROFILE = {'printing.print_preview_sticky_settings.appState': json.dumps(self._SETTINGS_SAVE_AS_PDF),
+                    "savefile.default_directory":  f"{DOWNLOAD_DIR}",
+                    "download.default_directory":  f"{DOWNLOAD_DIR}",
+                    "download.prompt_for_download": False,
+                    "download.directory_upgrade": True,
+                    "profile.managed_default_content_settings.images": 2,
+                    "safebrowsing.enabled": True}
+                
+            self._options.add_experimental_option('prefs', self._PROFILE)
+        
+        if headless == True:
+            self._options.add_argument('--headless')
+            
+        self._options.add_experimental_option("excludeSwitches", ["enable-logging", "enable-automation"])
+        self._options.add_experimental_option('useAutomationExtension', False)
+        self.user_agent = cria_user_agent()
+        self._options.add_argument(f"--user-agent=self.user_agent")
+        self._options.add_argument("--disable-web-security")
+        self._options.add_argument("--allow-running-insecure-content")
+        self._options.add_argument("--disable-extensions")
+        self._options.add_argument("--start-maximized")
+        self._options.add_argument("--no-sandbox")
+        self._options.add_argument("--disable-setuid-sandbox")
+        self._options.add_argument("--disable-infobars")
+        self._options.add_argument("--disable-webgl")
+        self._options.add_argument("--disable-popup-blocking")
+        self._options.add_argument('--disable-gpu')
+        self._options.add_argument('--disable-software-rasterizer')
+        self._options.add_argument('--no-proxy-server')
+        self._options.add_argument("--proxy-server='direct://'")
+        self._options.add_argument('--proxy-bypass-list=*')
+        self._options.add_argument('--disable-dev-shm-usage')
+        self._options.add_argument('--block-new-web-contents')
+        self._options.add_argument('--incognito')
+        self._options.add_argument('–disable-notifications')
+        self._options.add_argument("--window-size=1920,1080")
+        self._options.add_argument('--kiosk-printing')
+
+        
+        self.__service = Service(ChromeDriverManager().install())
+        
+        # create DRIVER
+        self.DRIVER = Chrome(service=self.__service, options=self._options)
+        
+        def enable_download_in_headless_chrome(driver, download_dir):
+            '''
+            Esse código adiciona suporte ao navegador Chrome sem interface gráfica (headless) no Selenium WebDriver para permitir o download automático de arquivos em um diretório especificado.
+
+            Mais especificamente, o código adiciona um comando ausente "send_command" ao executor de comando do driver e, em seguida, executa um comando "Page.setDownloadBehavior" para permitir o download automático de arquivos no diretório especificado.
+
+            O primeiro passo é necessário porque o suporte para o comando "send_command" não está incluído no Selenium WebDriver por padrão. O segundo passo usa o comando "Page.setDownloadBehavior" do Chrome DevTools Protocol para permitir o download automático de arquivos em um diretório especificado.
+
+            Em resumo, o código adiciona suporte para o download automático de arquivos em um diretório especificado no Chrome sem interface gráfica usando o Selenium WebDriver.
+            '''
+            driver.command_executor._commands["send_command"] = ("POST", '/session/$sessionId/chromium/send_command')
+
+            params = {'cmd': 'Page.setDownloadBehavior', 'params': {'behavior': 'allow', 'downloadPath': download_dir}}
+            command_result = driver.execute("send_command", params)
+        enable_download_in_headless_chrome(self.DRIVER, DOWNLOAD_DIR)
+        
+        
+        self.WDW3 = WebDriverWait(self.DRIVER, timeout=3)
+        self.WDW5 = WebDriverWait(self.DRIVER, timeout=5)
+        self.WDW7 = WebDriverWait(self.DRIVER, timeout=7)
+        self.WDW10 = WebDriverWait(self.DRIVER, timeout=10)
+        self.WDW30 = WebDriverWait(self.DRIVER, timeout=30)
+        self.WDW = self.WDW7
+
+        self.DRIVER.maximize_window()
+        return self.DRIVER
+
+esse código abaixo deve ser escrito no app.py considere #INICIOAPP.PY e #FIMAPP.PY
+#INICIOAPP.PY
+DRAFT_USER
+#FIMAPP.PY
+
+sabendo que ele será executado no main.py, faça o código acima com base no main.py abaixo e me dê apenas o método run que ficará dentro da classe RobotClass:
+
+from src.app.app import *
+
+if __name__ == '__main__':
+    app = RobotClass()
+    app.run()
+
+PRESTE MUITA ATENÇAO ABAIXO:
+NAO ME RESPONDA NADA MAIS QUE O CÓDIGO DO MÉTODO run()
+"""
```

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-6.1.0/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.0.2
+Version: 6.1.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
@@ -27,16 +27,15 @@
 
 ## Instalacao
 
 pip install FuncsForSPO em seu ambiente virtual e pronto!
 
 Powered By [https://github.com/gabriellopesdesouza2002](https://github.com/gabriellopesdesouza2002)
 
-
-# Current Version -> 4.35.0
+# Current Version -> 6.0.2
 
 version==4.33.1 -> Melhoria e criação de diversas funções desde a versão 4.24
 
 version==4.24.0 -> Melhoria nas documentações das funções, e melhoria na função de esperar elemento
 
  version==4.23.6 -> Melhoria nas documentações das funções, e adicionada uma função para ver dias a frente ou dias a atrás
```

### Comparing `FuncsForSPO-6.0.2/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-6.1.0/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 FuncsForSPO/femails/femails.py
 FuncsForSPO/fexceptions/__init__.py
 FuncsForSPO/fexceptions/exceptions.py
 FuncsForSPO/fftp/__init__.py
 FuncsForSPO/fftp/fftp.py
 FuncsForSPO/flanguage/__init__.py
 FuncsForSPO/flanguage/translator/__init__.py
+FuncsForSPO/flanguage/translator/__translator.py
+FuncsForSPO/flanguage/translator/base.py
 FuncsForSPO/flanguage/translator/translator.py
 FuncsForSPO/fopenpyxl/__init__.py
 FuncsForSPO/fopenpyxl/openpyxl_funcs.py
 FuncsForSPO/fpdf/__init__.py
 FuncsForSPO/fpdf/fanalyser/__init__.py
 FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
 FuncsForSPO/fpdf/fanalyser/base.py
```

### Comparing `FuncsForSPO-6.0.2/LICENSE` & `FuncsForSPO-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.2/PKG-INFO` & `FuncsForSPO-6.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.0.2
+Version: 6.1.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
@@ -27,16 +27,15 @@
 
 ## Instalacao
 
 pip install FuncsForSPO em seu ambiente virtual e pronto!
 
 Powered By [https://github.com/gabriellopesdesouza2002](https://github.com/gabriellopesdesouza2002)
 
-
-# Current Version -> 4.35.0
+# Current Version -> 6.0.2
 
 version==4.33.1 -> Melhoria e criação de diversas funções desde a versão 4.24
 
 version==4.24.0 -> Melhoria nas documentações das funções, e melhoria na função de esperar elemento
 
  version==4.23.6 -> Melhoria nas documentações das funções, e adicionada uma função para ver dias a frente ou dias a atrás
```

### Comparing `FuncsForSPO-6.0.2/README.md` & `FuncsForSPO-6.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 
 ## Instalacao
 
 pip install FuncsForSPO em seu ambiente virtual e pronto!
 
 Powered By [https://github.com/gabriellopesdesouza2002](https://github.com/gabriellopesdesouza2002)
 
-
-# Current Version -> 4.35.0
+# Current Version -> 6.0.2
 
 version==4.33.1 -> Melhoria e criação de diversas funções desde a versão 4.24
 
 version==4.24.0 -> Melhoria nas documentações das funções, e melhoria na função de esperar elemento
 
  version==4.23.6 -> Melhoria nas documentações das funções, e adicionada uma função para ver dias a frente ou dias a atrás
```

### Comparing `FuncsForSPO-6.0.2/setup.py` & `FuncsForSPO-6.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '6.0.2'
+version = '6.1.0'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

