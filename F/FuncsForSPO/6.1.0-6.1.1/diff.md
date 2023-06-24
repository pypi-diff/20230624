# Comparing `tmp/FuncsForSPO-6.1.0.tar.gz` & `tmp/FuncsForSPO-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-6.1.0.tar", last modified: Sat Jun 24 21:18:55 2023, max compression
+gzip compressed data, was "FuncsForSPO-6.1.1.tar", last modified: Sat Jun 24 21:21:29 2023, max compression
```

## Comparing `FuncsForSPO-6.1.0.tar` & `FuncsForSPO-6.1.1.tar`

### file list

```diff
@@ -1,80 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.457711 FuncsForSPO-6.1.0/
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.073004 FuncsForSPO-6.1.0/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.134342 FuncsForSPO-6.1.0/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.1.0/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.1.0/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.145359 FuncsForSPO-6.1.0/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.0/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.1.0/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.155949 FuncsForSPO-6.1.0/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.0/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.1.0/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.160476 FuncsForSPO-6.1.0/FuncsForSPO/flanguage/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.0/FuncsForSPO/flanguage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.178476 FuncsForSPO-6.1.0/FuncsForSPO/flanguage/translator/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.0/FuncsForSPO/flanguage/translator/__init__.py
--rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.1.0/FuncsForSPO/flanguage/translator/__translator.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.0/FuncsForSPO/flanguage/translator/base.py
--rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.1.0/FuncsForSPO/flanguage/translator/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.190479 FuncsForSPO-6.1.0/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.0/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.1.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.195475 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.230527 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0     8203 2023-06-19 21:37:07.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
--rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
--rw-rw-rw-   0        0        0     1340 2023-06-17 20:27:40.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.250535 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.267068 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.274070 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.303074 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/base.py
--rw-rw-rw-   0        0        0     8971 2023-06-18 22:41:54.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.316130 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.326126 FuncsForSPO-6.1.0/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.337127 FuncsForSPO-6.1.0/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    69692 2023-06-24 21:18:37.000000 FuncsForSPO-6.1.0/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.348133 FuncsForSPO-6.1.0/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.0/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.1.0/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.362687 FuncsForSPO-6.1.0/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.0/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39083 2023-06-06 21:05:50.000000 FuncsForSPO-6.1.0/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.374694 FuncsForSPO-6.1.0/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.0/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.1.0/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.384683 FuncsForSPO-6.1.0/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.1.0/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.1.0/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.390684 FuncsForSPO-6.1.0/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.1.0/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:18:55.124353 FuncsForSPO-6.1.0/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8023 2023-06-24 21:18:54.000000 FuncsForSPO-6.1.0/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1976 2023-06-24 21:18:54.000000 FuncsForSPO-6.1.0/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 21:18:54.000000 FuncsForSPO-6.1.0/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-06-24 21:18:54.000000 FuncsForSPO-6.1.0/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      458 2023-06-24 21:18:54.000000 FuncsForSPO-6.1.0/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.1.0/LICENSE
--rw-rw-rw-   0        0        0     8023 2023-06-24 21:18:55.454168 FuncsForSPO-6.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 21:18:55.457711 FuncsForSPO-6.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2611 2023-06-24 21:16:16.000000 FuncsForSPO-6.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.947786 FuncsForSPO-6.1.1/
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.525601 FuncsForSPO-6.1.1/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.582229 FuncsForSPO-6.1.1/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.1.1/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.1.1/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.593208 FuncsForSPO-6.1.1/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.1/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.1.1/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.605225 FuncsForSPO-6.1.1/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.1/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.1.1/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.622760 FuncsForSPO-6.1.1/FuncsForSPO/fgpt/
+-rw-rw-rw-   0        0        0      886 2023-06-24 20:49:12.000000 FuncsForSPO-6.1.1/FuncsForSPO/fgpt/__fgpt.py
+-rw-rw-rw-   0        0        0        0 2023-06-24 21:16:46.000000 FuncsForSPO-6.1.1/FuncsForSPO/fgpt/__init__.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.1.1/FuncsForSPO/fgpt/base.py
+-rw-rw-rw-   0        0        0      621 2023-06-24 21:16:37.000000 FuncsForSPO-6.1.1/FuncsForSPO/fgpt/fgpt.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.627754 FuncsForSPO-6.1.1/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.1/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.646757 FuncsForSPO-6.1.1/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.1.1/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.1.1/FuncsForSPO/flanguage/translator/__translator.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.1/FuncsForSPO/flanguage/translator/base.py
+-rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.1.1/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.659458 FuncsForSPO-6.1.1/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.1/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.1.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.667457 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.701319 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0     8203 2023-06-19 21:37:07.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
+-rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
+-rw-rw-rw-   0        0        0     1340 2023-06-17 20:27:40.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.723868 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.741475 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.746481 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.776108 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/base.py
+-rw-rw-rw-   0        0        0     8971 2023-06-18 22:41:54.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.787106 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.799909 FuncsForSPO-6.1.1/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.809507 FuncsForSPO-6.1.1/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    69692 2023-06-24 21:18:37.000000 FuncsForSPO-6.1.1/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.822045 FuncsForSPO-6.1.1/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.1/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.1.1/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.833044 FuncsForSPO-6.1.1/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.1/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39083 2023-06-06 21:05:50.000000 FuncsForSPO-6.1.1/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.864039 FuncsForSPO-6.1.1/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.1.1/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.1.1/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.873162 FuncsForSPO-6.1.1/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.1.1/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.1.1/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.879167 FuncsForSPO-6.1.1/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.1.1/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:21:29.571695 FuncsForSPO-6.1.1/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8023 2023-06-24 21:21:29.000000 FuncsForSPO-6.1.1/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2082 2023-06-24 21:21:29.000000 FuncsForSPO-6.1.1/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 21:21:29.000000 FuncsForSPO-6.1.1/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-06-24 21:21:29.000000 FuncsForSPO-6.1.1/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      475 2023-06-24 21:21:29.000000 FuncsForSPO-6.1.1/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.1.1/LICENSE
+-rw-rw-rw-   0        0        0     8023 2023-06-24 21:21:29.943781 FuncsForSPO-6.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 21:21:29.947786 FuncsForSPO-6.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2661 2023-06-24 21:21:23.000000 FuncsForSPO-6.1.1/setup.py
```

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/femails/femails.py` & `FuncsForSPO-6.1.1/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/flanguage/translator/__translator.py` & `FuncsForSPO-6.1.1/FuncsForSPO/flanguage/translator/__translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/flanguage/translator/base.py` & `FuncsForSPO-6.1.1/FuncsForSPO/flanguage/translator/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/flanguage/translator/translator.py` & `FuncsForSPO-6.1.1/FuncsForSPO/flanguage/translator/translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fgpt/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/__ocr_online_v2.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/__ocr_online_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/base.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpdf/pdfutils/pdfutils.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-6.1.1/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO/utils/utils.py` & `FuncsForSPO-6.1.1/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-6.1.1/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.1.0
+Version: 6.1.1
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.1.0/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-6.1.1/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 FuncsForSPO.egg-info/top_level.txt
 FuncsForSPO/femails/__init__.py
 FuncsForSPO/femails/femails.py
 FuncsForSPO/fexceptions/__init__.py
 FuncsForSPO/fexceptions/exceptions.py
 FuncsForSPO/fftp/__init__.py
 FuncsForSPO/fftp/fftp.py
+FuncsForSPO/fgpt/__fgpt.py
+FuncsForSPO/fgpt/__init__.py
+FuncsForSPO/fgpt/base.py
+FuncsForSPO/fgpt/fgpt.py
 FuncsForSPO/flanguage/__init__.py
 FuncsForSPO/flanguage/translator/__init__.py
 FuncsForSPO/flanguage/translator/__translator.py
 FuncsForSPO/flanguage/translator/base.py
 FuncsForSPO/flanguage/translator/translator.py
 FuncsForSPO/fopenpyxl/__init__.py
 FuncsForSPO/fopenpyxl/openpyxl_funcs.py
```

### Comparing `FuncsForSPO-6.1.0/LICENSE` & `FuncsForSPO-6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/PKG-INFO` & `FuncsForSPO-6.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.1.0
+Version: 6.1.1
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.1.0/README.md` & `FuncsForSPO-6.1.1/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.1.0/setup.py` & `FuncsForSPO-6.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '6.1.0'
+version = '6.1.1'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
@@ -15,14 +15,15 @@
         long_description_content_type="text/markdown",
         author_email='githubpaycon@gmail.com',
         keywords='Funções Para Melhorar Desenvolvimento de Robôs com Selenium',
         description=u'Funções Para Melhorar Desenvolvimento de Robôs com Selenium',
         
         packages= [
             os.path.join('FuncsForSPO', 'femails'),
+            os.path.join('FuncsForSPO', 'fgpt'),
             os.path.join('FuncsForSPO', 'fexceptions'),
             os.path.join('FuncsForSPO', 'fftp'),
             os.path.join('FuncsForSPO', 'flanguage'),
             os.path.join('FuncsForSPO', 'flanguage', 'translator'),
             os.path.join('FuncsForSPO', 'fpdf'),
             os.path.join('FuncsForSPO', 'fpdf', 'focr'),
             os.path.join('FuncsForSPO', 'fpdf', 'focr'),
```

