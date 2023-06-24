# Comparing `tmp/mc3-3.1.2.tar.gz` & `tmp/mc3-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mc3-3.1.2.tar", last modified: Sun Apr  9 14:49:19 2023, max compression
+gzip compressed data, was "mc3-3.1.3.tar", last modified: Sat Jun 24 15:32:17 2023, max compression
```

## Comparing `mc3-3.1.2.tar` & `mc3-3.1.3.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.118392 mc3-3.1.2/
--rw-r--r--   0 pato       (501) staff       (20)      123 2023-03-30 17:50:12.000000 mc3-3.1.2/.readthedocs.yml
--rw-r--r--   0 pato       (501) staff       (20)     2943 2022-03-19 12:17:57.000000 mc3-3.1.2/CONTRIBUTING.md
--rw-r--r--   0 pato       (501) staff       (20)     1085 2022-03-19 12:17:57.000000 mc3-3.1.2/LICENSE
--rw-r--r--   0 pato       (501) staff       (20)      402 2022-03-19 12:17:57.000000 mc3-3.1.2/MANIFEST.in
--rw-r--r--   0 pato       (501) staff       (20)      991 2022-03-19 12:17:57.000000 mc3-3.1.2/Makefile
--rw-r--r--   0 pato       (501) staff       (20)     2422 2023-04-09 14:49:19.118268 mc3-3.1.2/PKG-INFO
--rw-r--r--   0 pato       (501) staff       (20)     1779 2023-04-04 14:34:51.000000 mc3-3.1.2/README.md
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.108868 mc3-3.1.2/docs/
--rw-r--r--   0 pato       (501) staff       (20)     7657 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/Makefile
--rw-r--r--   0 pato       (501) staff       (20)    62757 2023-03-30 17:50:12.000000 mc3-3.1.2/docs/api.rst
--rw-r--r--   0 pato       (501) staff       (20)    11541 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/conf.py
--rw-r--r--   0 pato       (501) staff       (20)     2970 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/contributing.rst
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.110961 mc3-3.1.2/docs/figures/
--rw-r--r--   0 pato       (501) staff       (20)    32125 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/figures/quad_bestfit.png
--rw-r--r--   0 pato       (501) staff       (20)    34319 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/figures/quad_fitting.png
--rw-r--r--   0 pato       (501) staff       (20)    46027 2023-03-30 13:26:40.000000 mc3-3.1.2/docs/figures/quad_hist.png
--rw-r--r--   0 pato       (501) staff       (20)   242288 2023-03-30 13:26:40.000000 mc3-3.1.2/docs/figures/quad_pairwise.png
--rw-r--r--   0 pato       (501) staff       (20)   211712 2023-03-30 13:26:40.000000 mc3-3.1.2/docs/figures/quad_trace.png
--rw-r--r--   0 pato       (501) staff       (20)    48970 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/figures/rms-vs-binsize.png
--rw-r--r--   0 pato       (501) staff       (20)     8854 2023-03-30 13:26:40.000000 mc3-3.1.2/docs/fit_tutorial.rst
--rw-r--r--   0 pato       (501) staff       (20)     6915 2023-04-09 14:48:51.000000 mc3-3.1.2/docs/get_started.rst
--rw-r--r--   0 pato       (501) staff       (20)     4370 2023-04-04 14:34:51.000000 mc3-3.1.2/docs/index.rst
--rw-r--r--   0 pato       (501) staff       (20)     1140 2023-03-30 13:26:40.000000 mc3-3.1.2/docs/license.rst
--rw-r--r--   0 pato       (501) staff       (20)     7243 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/make.bat
--rw-r--r--   0 pato       (501) staff       (20)    28030 2023-03-30 13:26:40.000000 mc3-3.1.2/docs/mcmc_tutorial.rst
--rw-r--r--   0 pato       (501) staff       (20)     1691 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/references.rst
--rw-r--r--   0 pato       (501) staff       (20)     1333 2022-03-19 12:17:57.000000 mc3-3.1.2/docs/time_averaging.rst
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.111862 mc3-3.1.2/examples/
--rw-r--r--   0 pato       (501) staff       (20)     1650 2023-03-30 13:26:40.000000 mc3-3.1.2/examples/get_started.py
--rw-r--r--   0 pato       (501) staff       (20)     2243 2022-03-19 12:17:57.000000 mc3-3.1.2/examples/ns_tutorial.py
--rw-r--r--   0 pato       (501) staff       (20)     1556 2022-03-19 12:17:57.000000 mc3-3.1.2/examples/timeavg.py
--rw-r--r--   0 pato       (501) staff       (20)     2792 2023-03-30 13:26:40.000000 mc3-3.1.2/examples/tutorial.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.113476 mc3-3.1.2/mc3/
--rw-r--r--   0 pato       (501) staff       (20)      688 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)    10937 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/__main__.py
--rw-r--r--   0 pato       (501) staff       (20)    13086 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/chain.py
--rw-r--r--   0 pato       (501) staff       (20)     9288 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/fit_driver.py
--rw-r--r--   0 pato       (501) staff       (20)    13642 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/mcmc_driver.py
--rw-r--r--   0 pato       (501) staff       (20)     6544 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/ns_driver.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.114900 mc3-3.1.2/mc3/plots/
--rw-r--r--   0 pato       (501) staff       (20)      604 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/plots/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)     5594 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/plots/colors.py
--rw-r--r--   0 pato       (501) staff       (20)    10671 2023-03-30 17:50:12.000000 mc3-3.1.2/mc3/plots/plot_functions.py
--rw-r--r--   0 pato       (501) staff       (20)    39119 2023-04-09 14:48:51.000000 mc3-3.1.2/mc3/plots/posterior.py
--rw-r--r--   0 pato       (501) staff       (20)    15233 2023-03-30 13:16:39.000000 mc3-3.1.2/mc3/sampler.py
--rw-r--r--   0 pato       (501) staff       (20)    24594 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/sampler_driver.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.115976 mc3-3.1.2/mc3/stats/
--rw-r--r--   0 pato       (501) staff       (20)      638 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/stats/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)     2674 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/stats/gelman.py
--rw-r--r--   0 pato       (501) staff       (20)      811 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/stats/prayer.py
--rw-r--r--   0 pato       (501) staff       (20)    35522 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/stats/stats.py
--rw-r--r--   0 pato       (501) staff       (20)     1589 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/stats/time_averaging.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.116365 mc3-3.1.2/mc3/utils/
--rw-r--r--   0 pato       (501) staff       (20)      529 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/utils/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)     7119 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/utils/log.py
--rw-r--r--   0 pato       (501) staff       (20)    13722 2023-03-30 13:26:40.000000 mc3-3.1.2/mc3/utils/utils.py
--rw-r--r--   0 pato       (501) staff       (20)      275 2023-04-09 14:48:51.000000 mc3-3.1.2/mc3/version.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.114228 mc3-3.1.2/mc3.egg-info/
--rw-r--r--   0 pato       (501) staff       (20)     2422 2023-04-09 14:49:18.000000 mc3-3.1.2/mc3.egg-info/PKG-INFO
--rw-r--r--   0 pato       (501) staff       (20)     1460 2023-04-09 14:49:19.000000 mc3-3.1.2/mc3.egg-info/SOURCES.txt
--rw-r--r--   0 pato       (501) staff       (20)        1 2023-04-09 14:49:18.000000 mc3-3.1.2/mc3.egg-info/dependency_links.txt
--rw-r--r--   0 pato       (501) staff       (20)       43 2023-04-09 14:49:18.000000 mc3-3.1.2/mc3.egg-info/entry_points.txt
--rw-r--r--   0 pato       (501) staff       (20)       45 2023-04-09 14:49:18.000000 mc3-3.1.2/mc3.egg-info/requires.txt
--rw-r--r--   0 pato       (501) staff       (20)        4 2023-04-09 14:49:18.000000 mc3-3.1.2/mc3.egg-info/top_level.txt
--rw-r--r--   0 pato       (501) staff       (20)      144 2022-03-19 12:17:57.000000 mc3-3.1.2/pyproject.toml
--rw-r--r--   0 pato       (501) staff       (20)      150 2022-03-19 12:17:57.000000 mc3-3.1.2/pytest.ini
--rw-r--r--   0 pato       (501) staff       (20)       57 2023-03-30 17:50:12.000000 mc3-3.1.2/requirements.txt
--rw-r--r--   0 pato       (501) staff       (20)       38 2023-04-09 14:49:19.118433 mc3-3.1.2/setup.cfg
--rw-r--r--   0 pato       (501) staff       (20)     1721 2023-03-30 17:50:12.000000 mc3-3.1.2/setup.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.116858 mc3-3.1.2/src_c/
--rw-r--r--   0 pato       (501) staff       (20)     3973 2023-03-30 13:26:40.000000 mc3-3.1.2/src_c/_binarray.c
--rw-r--r--   0 pato       (501) staff       (20)     7667 2023-03-30 13:26:40.000000 mc3-3.1.2/src_c/_chisq.c
--rw-r--r--   0 pato       (501) staff       (20)    10514 2023-03-30 13:26:40.000000 mc3-3.1.2/src_c/_dwt.c
--rw-r--r--   0 pato       (501) staff       (20)     6902 2023-03-30 13:26:40.000000 mc3-3.1.2/src_c/_time_averaging.c
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.117215 mc3-3.1.2/src_c/include/
--rw-r--r--   0 pato       (501) staff       (20)      522 2023-03-30 13:26:40.000000 mc3-3.1.2/src_c/include/ind.h
--rw-r--r--   0 pato       (501) staff       (20)     6632 2023-03-30 13:26:40.000000 mc3-3.1.2/src_c/include/stats.h
--rw-r--r--   0 pato       (501) staff       (20)     4185 2023-03-30 13:26:40.000000 mc3-3.1.2/src_c/include/wavelet.h
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-04-09 14:49:19.118071 mc3-3.1.2/tests/
--rw-r--r--   0 pato       (501) staff       (20)     5592 2023-03-30 13:26:40.000000 mc3-3.1.2/tests/test_dynesty.py
--rw-r--r--   0 pato       (501) staff       (20)     3988 2023-03-30 13:26:40.000000 mc3-3.1.2/tests/test_fit.py
--rw-r--r--   0 pato       (501) staff       (20)     2281 2023-03-30 13:26:40.000000 mc3-3.1.2/tests/test_logging.py
--rw-r--r--   0 pato       (501) staff       (20)    15975 2023-03-30 13:26:40.000000 mc3-3.1.2/tests/test_mcmc.py
--rw-r--r--   0 pato       (501) staff       (20)     3790 2023-03-30 13:26:40.000000 mc3-3.1.2/tests/test_plots.py
--rw-r--r--   0 pato       (501) staff       (20)    14911 2023-03-30 13:26:40.000000 mc3-3.1.2/tests/test_stats.py
--rw-r--r--   0 pato       (501) staff       (20)     8937 2023-03-30 13:26:40.000000 mc3-3.1.2/tests/test_utils.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.887901 mc3-3.1.3/
+-rw-r--r--   0 pato       (501) staff       (20)      123 2023-04-13 07:59:40.000000 mc3-3.1.3/.readthedocs.yml
+-rw-r--r--   0 pato       (501) staff       (20)     2943 2019-08-12 13:25:42.000000 mc3-3.1.3/CONTRIBUTING.md
+-rw-r--r--   0 pato       (501) staff       (20)     1085 2022-05-11 13:31:47.000000 mc3-3.1.3/LICENSE
+-rw-r--r--   0 pato       (501) staff       (20)      402 2022-05-11 13:31:47.000000 mc3-3.1.3/MANIFEST.in
+-rw-r--r--   0 pato       (501) staff       (20)      991 2019-08-12 13:25:42.000000 mc3-3.1.3/Makefile
+-rw-r--r--   0 pato       (501) staff       (20)     2422 2023-06-24 15:32:17.887760 mc3-3.1.3/PKG-INFO
+-rw-r--r--   0 pato       (501) staff       (20)     1779 2023-04-13 07:59:40.000000 mc3-3.1.3/README.md
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.875943 mc3-3.1.3/docs/
+-rw-r--r--   0 pato       (501) staff       (20)     7657 2019-08-12 13:25:42.000000 mc3-3.1.3/docs/Makefile
+-rw-r--r--   0 pato       (501) staff       (20)    62757 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/api.rst
+-rw-r--r--   0 pato       (501) staff       (20)    11541 2019-08-12 13:25:42.000000 mc3-3.1.3/docs/conf.py
+-rw-r--r--   0 pato       (501) staff       (20)     2970 2019-08-12 13:25:42.000000 mc3-3.1.3/docs/contributing.rst
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.877684 mc3-3.1.3/docs/figures/
+-rw-r--r--   0 pato       (501) staff       (20)    32125 2022-05-11 13:31:47.000000 mc3-3.1.3/docs/figures/quad_bestfit.png
+-rw-r--r--   0 pato       (501) staff       (20)    34319 2022-05-11 13:31:47.000000 mc3-3.1.3/docs/figures/quad_fitting.png
+-rw-r--r--   0 pato       (501) staff       (20)    46027 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/figures/quad_hist.png
+-rw-r--r--   0 pato       (501) staff       (20)   242288 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/figures/quad_pairwise.png
+-rw-r--r--   0 pato       (501) staff       (20)   211712 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/figures/quad_trace.png
+-rw-r--r--   0 pato       (501) staff       (20)    48970 2022-05-11 13:31:47.000000 mc3-3.1.3/docs/figures/rms-vs-binsize.png
+-rw-r--r--   0 pato       (501) staff       (20)     8854 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/fit_tutorial.rst
+-rw-r--r--   0 pato       (501) staff       (20)     6915 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/get_started.rst
+-rw-r--r--   0 pato       (501) staff       (20)     4370 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/index.rst
+-rw-r--r--   0 pato       (501) staff       (20)     1140 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/license.rst
+-rw-r--r--   0 pato       (501) staff       (20)     7243 2019-08-12 13:25:42.000000 mc3-3.1.3/docs/make.bat
+-rw-r--r--   0 pato       (501) staff       (20)    28030 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/mcmc_tutorial.rst
+-rw-r--r--   0 pato       (501) staff       (20)     1691 2019-08-12 13:25:42.000000 mc3-3.1.3/docs/references.rst
+-rw-r--r--   0 pato       (501) staff       (20)     1333 2022-05-11 13:31:47.000000 mc3-3.1.3/docs/time_averaging.rst
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.880246 mc3-3.1.3/examples/
+-rw-r--r--   0 pato       (501) staff       (20)     1650 2023-04-13 07:59:40.000000 mc3-3.1.3/examples/get_started.py
+-rw-r--r--   0 pato       (501) staff       (20)     2243 2019-08-12 13:25:42.000000 mc3-3.1.3/examples/ns_tutorial.py
+-rw-r--r--   0 pato       (501) staff       (20)     1148 2023-04-14 13:30:47.000000 mc3-3.1.3/examples/ppf.py
+-rw-r--r--   0 pato       (501) staff       (20)     1556 2019-08-12 13:25:42.000000 mc3-3.1.3/examples/timeavg.py
+-rw-r--r--   0 pato       (501) staff       (20)     2792 2023-04-13 07:59:40.000000 mc3-3.1.3/examples/tutorial.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.881518 mc3-3.1.3/mc3/
+-rw-r--r--   0 pato       (501) staff       (20)      688 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)    10937 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/__main__.py
+-rw-r--r--   0 pato       (501) staff       (20)    13086 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/chain.py
+-rw-r--r--   0 pato       (501) staff       (20)     9288 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/fit_driver.py
+-rw-r--r--   0 pato       (501) staff       (20)    13642 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/mcmc_driver.py
+-rw-r--r--   0 pato       (501) staff       (20)     6544 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/ns_driver.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.883076 mc3-3.1.3/mc3/plots/
+-rw-r--r--   0 pato       (501) staff       (20)      604 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/plots/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)     5594 2023-06-24 15:31:48.000000 mc3-3.1.3/mc3/plots/colors.py
+-rw-r--r--   0 pato       (501) staff       (20)    23328 2021-01-24 14:25:07.000000 mc3-3.1.3/mc3/plots/mc3_plots.py
+-rw-r--r--   0 pato       (501) staff       (20)    10671 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/plots/plot_functions.py
+-rw-r--r--   0 pato       (501) staff       (20)    39119 2023-06-02 12:30:58.000000 mc3-3.1.3/mc3/plots/posterior.py
+-rw-r--r--   0 pato       (501) staff       (20)    24594 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/sampler_driver.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.884992 mc3-3.1.3/mc3/stats/
+-rw-r--r--   0 pato       (501) staff       (20)      638 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/stats/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)     2674 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/stats/gelman.py
+-rw-r--r--   0 pato       (501) staff       (20)      811 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/stats/prayer.py
+-rw-r--r--   0 pato       (501) staff       (20)    36306 2023-06-24 15:31:48.000000 mc3-3.1.3/mc3/stats/stats.py
+-rw-r--r--   0 pato       (501) staff       (20)     1589 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/stats/time_averaging.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.885732 mc3-3.1.3/mc3/utils/
+-rw-r--r--   0 pato       (501) staff       (20)      529 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/utils/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)     7119 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/utils/log.py
+-rw-r--r--   0 pato       (501) staff       (20)    13722 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/utils/utils.py
+-rw-r--r--   0 pato       (501) staff       (20)      275 2023-06-24 15:31:48.000000 mc3-3.1.3/mc3/version.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.882142 mc3-3.1.3/mc3.egg-info/
+-rw-r--r--   0 pato       (501) staff       (20)     2422 2023-06-24 15:32:17.000000 mc3-3.1.3/mc3.egg-info/PKG-INFO
+-rw-r--r--   0 pato       (501) staff       (20)     1484 2023-06-24 15:32:17.000000 mc3-3.1.3/mc3.egg-info/SOURCES.txt
+-rw-r--r--   0 pato       (501) staff       (20)        1 2023-06-24 15:32:17.000000 mc3-3.1.3/mc3.egg-info/dependency_links.txt
+-rw-r--r--   0 pato       (501) staff       (20)       43 2023-06-24 15:32:17.000000 mc3-3.1.3/mc3.egg-info/entry_points.txt
+-rw-r--r--   0 pato       (501) staff       (20)       45 2023-06-24 15:32:17.000000 mc3-3.1.3/mc3.egg-info/requires.txt
+-rw-r--r--   0 pato       (501) staff       (20)        4 2023-06-24 15:32:17.000000 mc3-3.1.3/mc3.egg-info/top_level.txt
+-rw-r--r--   0 pato       (501) staff       (20)      144 2022-05-11 13:31:47.000000 mc3-3.1.3/pyproject.toml
+-rw-r--r--   0 pato       (501) staff       (20)      150 2019-08-12 13:25:42.000000 mc3-3.1.3/pytest.ini
+-rw-r--r--   0 pato       (501) staff       (20)       57 2023-04-13 07:59:40.000000 mc3-3.1.3/requirements.txt
+-rw-r--r--   0 pato       (501) staff       (20)       38 2023-06-24 15:32:17.887943 mc3-3.1.3/setup.cfg
+-rw-r--r--   0 pato       (501) staff       (20)     1728 2023-06-24 15:31:48.000000 mc3-3.1.3/setup.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.886260 mc3-3.1.3/src_c/
+-rw-r--r--   0 pato       (501) staff       (20)     3973 2023-04-13 07:59:40.000000 mc3-3.1.3/src_c/_binarray.c
+-rw-r--r--   0 pato       (501) staff       (20)     7667 2023-04-13 07:59:40.000000 mc3-3.1.3/src_c/_chisq.c
+-rw-r--r--   0 pato       (501) staff       (20)    10514 2023-04-13 07:59:40.000000 mc3-3.1.3/src_c/_dwt.c
+-rw-r--r--   0 pato       (501) staff       (20)     6902 2023-04-13 07:59:40.000000 mc3-3.1.3/src_c/_time_averaging.c
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.886631 mc3-3.1.3/src_c/include/
+-rw-r--r--   0 pato       (501) staff       (20)      522 2023-04-13 07:59:40.000000 mc3-3.1.3/src_c/include/ind.h
+-rw-r--r--   0 pato       (501) staff       (20)     6646 2023-06-24 15:31:48.000000 mc3-3.1.3/src_c/include/stats.h
+-rw-r--r--   0 pato       (501) staff       (20)     4185 2023-04-13 07:59:40.000000 mc3-3.1.3/src_c/include/wavelet.h
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.887547 mc3-3.1.3/tests/
+-rw-r--r--   0 pato       (501) staff       (20)     5592 2023-04-13 07:59:40.000000 mc3-3.1.3/tests/test_dynesty.py
+-rw-r--r--   0 pato       (501) staff       (20)     3988 2023-04-13 07:59:40.000000 mc3-3.1.3/tests/test_fit.py
+-rw-r--r--   0 pato       (501) staff       (20)     2281 2023-04-13 07:59:40.000000 mc3-3.1.3/tests/test_logging.py
+-rw-r--r--   0 pato       (501) staff       (20)    15975 2023-04-13 07:59:40.000000 mc3-3.1.3/tests/test_mcmc.py
+-rw-r--r--   0 pato       (501) staff       (20)     3790 2023-06-24 15:31:48.000000 mc3-3.1.3/tests/test_plots.py
+-rw-r--r--   0 pato       (501) staff       (20)    14911 2023-04-13 07:59:40.000000 mc3-3.1.3/tests/test_stats.py
+-rw-r--r--   0 pato       (501) staff       (20)     8937 2023-04-13 07:59:40.000000 mc3-3.1.3/tests/test_utils.py
```

### Comparing `mc3-3.1.2/CONTRIBUTING.md` & `mc3-3.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/LICENSE` & `mc3-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/Makefile` & `mc3-3.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/PKG-INFO` & `mc3-3.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mc3
-Version: 3.1.2
+Version: 3.1.3
 Summary: Multi-core Markov-chain Monte Carlo package.
 Home-page: https://github.com/pcubillos/mc3
 Author: Patricio Cubillos
 Author-email: patricio.cubillos@oeaw.ac.at
 License: MIT
 Description: # mc3: Multi-core Markov-chain Monte Carlo
         > A Python implementation of the Markov-chain Monte Carlo algorithm.
```

### Comparing `mc3-3.1.2/README.md` & `mc3-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/Makefile` & `mc3-3.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/api.rst` & `mc3-3.1.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/conf.py` & `mc3-3.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/contributing.rst` & `mc3-3.1.3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/figures/quad_bestfit.png` & `mc3-3.1.3/docs/figures/quad_bestfit.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/figures/quad_fitting.png` & `mc3-3.1.3/docs/figures/quad_fitting.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/figures/quad_hist.png` & `mc3-3.1.3/docs/figures/quad_hist.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/figures/quad_pairwise.png` & `mc3-3.1.3/docs/figures/quad_pairwise.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/figures/quad_trace.png` & `mc3-3.1.3/docs/figures/quad_trace.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/figures/rms-vs-binsize.png` & `mc3-3.1.3/docs/figures/rms-vs-binsize.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/fit_tutorial.rst` & `mc3-3.1.3/docs/fit_tutorial.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/get_started.rst` & `mc3-3.1.3/docs/get_started.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/index.rst` & `mc3-3.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/license.rst` & `mc3-3.1.3/docs/license.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/make.bat` & `mc3-3.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/mcmc_tutorial.rst` & `mc3-3.1.3/docs/mcmc_tutorial.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/references.rst` & `mc3-3.1.3/docs/references.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/docs/time_averaging.rst` & `mc3-3.1.3/docs/time_averaging.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/examples/get_started.py` & `mc3-3.1.3/examples/get_started.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/examples/ns_tutorial.py` & `mc3-3.1.3/examples/ns_tutorial.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/examples/timeavg.py` & `mc3-3.1.3/examples/timeavg.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/examples/tutorial.py` & `mc3-3.1.3/examples/tutorial.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3/__init__.py` & `mc3-3.1.3/mc3/__init__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3/__main__.py` & `mc3-3.1.3/mc3/__main__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3/chain.py` & `mc3-3.1.3/mc3/chain.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3/fit_driver.py` & `mc3-3.1.3/mc3/fit_driver.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3/mcmc_driver.py` & `mc3-3.1.3/mc3/mcmc_driver.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3/ns_driver.py` & `mc3-3.1.3/mc3/ns_driver.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3/plots/__init__.py` & `mc3-3.1.3/mc3/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3/plots/colors.py` & `mc3-3.1.3/mc3/plots/colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         ex = fig.dpi_scale_trans.inverted().transform_bbox(ex)
         t = text.get_transform() + offset_copy(Affine2D(), fig=fig, y=ex.height)
     return printed_texts
 
 
 class Theme():
     """A monochromatic color theme from given color"""
-    def __init__(self, color, alpha_light=0.15, alpha_dark=0.5):
+    def __init__(self, color, alpha_light=0.15, alpha_dark=0.7):
         """
         Parameters
         ----------
         color: color or iterable of colors
             The color to alphatize.
         alpha_light: Float
             Alpha color value to merge with white to make self.light_color.
```

### Comparing `mc3-3.1.2/mc3/plots/plot_functions.py` & `mc3-3.1.3/mc3/plots/plot_functions.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3/plots/posterior.py` & `mc3-3.1.3/mc3/plots/posterior.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3/sampler.py` & `mc3-3.1.3/mc3/utils/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,386 +1,470 @@
-class sampler():
-    def __init__(
-        self, data=None, uncert=None, func=None, params=None, indparams=[],
-        pmin=None, pmax=None, pstep=None,
-        prior=None, priorlow=None, priorup=None,
-        sampler=None, ncpu=None, leastsq=None, chisqscale=False,
-        nchains=7, nsamples=None, burnin=0, thinning=1,
-        grtest=True, grbreak=0.0, grnmin=0.5, wlike=False,
-        fgamma=1.0, fepsilon=0.0, hsize=10, kickoff='normal',
-        plots=False, ioff=False, showbp=True, savefile=None, resume=False,
-        rms=False, log=None, pnames=None, texnames=None,
-        **kwargs,
+# Copyright (c) 2015-2023 Patricio Cubillos and contributors.
+# mc3 is open-source software under the MIT license (see LICENSE).
+
+__all__ = [
+    'ROOT',
+    'parray',
+    'saveascii',
+    'loadascii',
+    'savebin',
+    'loadbin',
+    'isfile',
+    'burn',
+    'default_parnames',
+    'tex_parameters',
+]
+
+from decimal import Decimal
+import os
+
+import numpy as np
+
+ROOT = os.path.realpath(os.path.dirname(__file__) + '/../..') + '/'
+
+
+def parray(string):
+    """
+    Convert a string containin a list of white-space-separated (and/or
+    newline-separated) values into a numpy array
+    """
+    if string == 'None':
+        return None
+    try:    # If they can be converted into doubles, do it:
+        return np.asarray(string.split(), np.double)
+    except: # Else, return a string array:
+        return string.split()
+
+
+def saveascii(data, filename, precision=8):
+    """
+    Write (numeric) data to ASCII file.
+
+    Parameters
+    ----------
+    data:  1D/2D numeric iterable (ndarray, list, tuple, or combination)
+        Data to be stored in file.
+    filename:  String
+        File where to store the arrlist.
+    precision: Integer
+        Maximum number of significant digits of values.
+
+    Example
+    -------
+    >>> import numpy as np
+    >>> import mc3.utils as mu
+
+    >>> a = np.arange(4) * np.pi
+    >>> b = np.arange(4)
+    >>> c = np.logspace(0, 12, 4)
+
+    >>> outfile = 'delete.me'
+    >>> mu.saveascii([a,b,c], outfile)
+
+    >>> # This will produce this file:
+    >>> with open(outfile) as f:
+    >>>   print(f.read())
+            0         0         1
+    3.1415927         1     10000
+    6.2831853         2     1e+08
+     9.424778         3     1e+12
+    """
+    # Force it to be a 2D ndarray:
+    data = np.array(data, ndmin=2).T
+
+    # Save arrays to ASCII file:
+    with open(filename, 'w') as f:
+        for parvals in data:
+            f.write(' '.join(f'{v:9.{precision:d}g}' for v in parvals) + '\n')
+
+
+def loadascii(filename):
+    """
+    Extract data from file and store in a 2D ndarray (or list of arrays
+    if not square).  Blank or comment lines are ignored.
+
+    Parameters
+    ----------
+    filename: String
+        Name of file containing the data to read.
+
+    Returns
+    -------
+    array: 2D ndarray or list
+        See parameters description.
+    """
+    # Open and read the file:
+    lines = []
+    for line in open(filename, 'r'):
+        if not line.startswith('#') and line.strip() != '':
+            lines.append(line)
+
+    # Count number of lines:
+    npars = len(lines)
+
+    # Extract values:
+    ncolumns = len(lines[0].split())
+    array = np.zeros((npars, ncolumns), np.double)
+    for i, line in enumerate(lines):
+        array[i] = line.strip().split()
+    array = np.transpose(array)
+
+    return array
+
+
+def savebin(data, filename):
+    """
+    Write data variables into a numpy npz file.
+
+    Parameters
+    ----------
+    data:  List of data objects
+        Data to be stored in file.  Each array must have the same length.
+    filename:  String
+        File where to store the arrlist.
+
+    Note
+    ----
+    This wrapper around np.savez() preserves the data type of list and
+    tuple variables when the file is open with loadbin().
+
+    Example
+    -------
+    >>> import mc3.utils as mu
+    >>> import numpy as np
+    >>> # Save list of data variables to file:
+    >>> datafile = 'datafile.npz'
+    >>> indata = [np.arange(4), 'one', np.ones((2,2)), True, [42], (42, 42)]
+    >>> mu.savebin(indata, datafile)
+    >>> # Now load the file:
+    >>> outdata = mu.loadbin(datafile)
+    >>> for data in outdata:
+    >>>     print(repr(data))
+    array([0, 1, 2, 3])
+    'one'
+    array([[ 1.,  1.],
+           [ 1.,  1.]])
+    True
+    [42]
+    (42, 42)
+    """
+    # Get the number of elements to determine the key's fmt:
+    ndata = len(data)
+    fmt = len(str(ndata))
+
+    key = []
+    for i, datum in enumerate(data):
+        dkey = 'file{:{}d}'.format(i, fmt)
+        # Encode in the key if a variable is a list or tuple:
+        if isinstance(datum, list):
+            dkey += '_list'
+        elif isinstance(datum, tuple):
+            dkey += '_tuple'
+        elif isinstance(datum, str):
+            dkey += '_str'
+        elif isinstance(datum, bool):
+            dkey += '_bool'
+        key.append(dkey)
+
+    # Use a dictionary so savez() include the keys for each item:
+    d = dict(zip(key, data))
+    np.savez(filename, **d)
+
+
+def loadbin(filename):
+    """
+    Read a binary npz array, casting list and tuple variables into
+    their original data types.
+
+    Parameters
+    ----------
+    filename: String
+       Path to file containing the data to be read.
+
+    Return
+    ------
+    data:  List
+       List of objects stored in the file.
+
+    Example
+    -------
+    See example in savebin().
+    """
+    # Unpack data:
+    npz = np.load(filename)
+    data = []
+    for key, val in sorted(npz.items()):
+        data.append(val[()])
+        # Check if val is a str, bool, list, or tuple:
+        if '_' in key:
+            exec('data[-1] = ' + key[key.find('_')+1:] + '(data[-1])')
+
+    return data
+
+
+def isfile(input, iname, log, dtype, unpack=True, not_none=False):
+    """
+    Check if an input is a file name; if it is, read it.
+    Genereate error messages if it is the case.
+
+    Parameters
+    ----------
+    input: Iterable or String
+        The input variable.
+    iname: String
+        Input-variable name.
+    log: File pointer
+         If not None, print message to the given file pointer.
+    dtype: String
+        File data type, choose between 'bin' or 'ascii'.
+    unpack: Bool
+        If True, return the first element of a read file.
+    not_none: Bool
+        If True, throw an error if input is None.
+    """
+    # Set the loading function depending on the data type:
+    if dtype == 'bin':
+        load = loadbin
+    elif dtype == 'ascii':
+        load = loadascii
+    else:
+        log.error(
+            f"Invalid data type '{dtype}', must be either 'bin' or 'ascii'",
+        )
+
+    # Check if the input is None, throw error if requested:
+    if input is None:
+        if not_none:
+            log.error(f"'{iname}' is a required argument")
+        return None
+
+    # Check that it is an iterable:
+    if not np.iterable(input):
+        log.error(f'{iname} must be an iterable or a file name')
+
+    # Check if it is a string, a string in a list, or an array:
+    if isinstance(input, str):
+        ifile = input
+    elif isinstance(input[0], str):
+        ifile = input[0]
+    else:
+        return input
+
+    # It is a file name:
+    if not os.path.isfile(ifile):
+        log.error(f"{iname} file '{ifile}' not found")
+    if unpack:  # Unpack (remove outer dimension) if necessary
+        return load(ifile)[0]
+    return load(ifile)
+
+
+def burn(Zdict=None, burnin=None, Z=None, zchain=None, sort=True):
+    """
+    Return a posterior distribution removing the burnin initial iterations
+    of each chain from the input distribution.
+
+    Parameters
+    ----------
+    Zdict: dict
+        A dictionary (as in mc3's output) containing a posterior distribution
+        (Z) and number of iterations to burn (burnin).
+    burnin: Integer
+        Number of iterations to remove from the start of each chain.
+        If specified, it overrides value from Zdict.
+    Z: 2D float ndarray
+        Posterior distribution (of shape [nsamples,npars]) to consider
+        if Zdict is None.
+    zchain: 1D integer ndarray
+        Chain indices for the samples in Z (used only of Zdict is None).
+    sort: Bool
+        If True, sort the outputs by chain index.
+
+    Returns
+    -------
+    posterior: 2D float ndarray
+        Burned posterior distribution.
+    zchain: 1D integer ndarray
+        Burned zchain array.
+    zmask: 1D integer ndarray
+        Indices that transform Z into posterior.
+
+    Examples
+    --------
+    >>> import mc3.utils as mu
+    >>> import numpy as np
+    >>> # Mock a posterior-distribution output:
+    >>> Z = np.expand_dims([0., 1, 10, 20, 30, 11, 31, 21, 12, 22, 32], axis=1)
+    >>> zchain = np.array([-1, -1, 0, 1, 2, 0, 2, 1, 0, 1, 2])
+    >>> Zdict = {'posterior':Z, 'zchain':zchain, 'burnin':1}
+    >>> # Simply apply burn() into the dict:
+    >>> posterior, zchain, zmask = mu.burn(Zdict)
+    >>> print(posterior[:,0])
+    [11. 12. 21. 22. 31. 32.]
+    >>> print(zchain)
+    [0 0 1 1 2 2]
+    >>> print(zmask)
+    [ 5  8  7  9  6 10]
+    >>> # Samples were sorted by chain index, but one can prevent with:
+    >>> posterior, zchain, zmask = mu.burn(Zdict, sort=False)
+    >>> print(posterior[:,0])
+    [11. 31. 21. 12. 22. 32.]
+    >>> # One can also override the burn-in samples:
+    >>> posterior, zchain, zmask = mu.burn(Zdict, burnin=0)
+    >>> print(posterior[:,0])
+    [10. 11. 12. 20. 21. 22. 30. 31. 32.]
+    >>> # Or apply directly to arrays:
+    >>> posterior, zchain, zmask = mu.burn(Z=Z, zchain=zchain, burnin=1)
+    >>> print(posterior[:,0])
+    [11. 12. 21. 22. 31. 32.]
+    """
+    if Zdict is None and (Z is None or zchain is None or burnin is None):
+        raise ValueError(
+            'Need to input either Zdict or all three of burnin, Z, and zchain')
+    if Zdict is not None:
+        Z = Zdict['posterior']
+        zchain = Zdict['zchain']
+
+    if burnin is None:
+        burnin = Zdict['burnin']
+
+    mask = np.zeros_like(zchain, bool)
+    nchains = np.amax(zchain) + 1
+    for c in range(nchains):
+        mask[np.where(zchain == c)[0][burnin:]] = True
+
+    if sort:
+        zsort = np.lexsort([zchain])
+        zmask = zsort[np.where(mask[zsort])]
+    else:
+        zmask = np.where(mask)[0]
+
+    # Values accepted for posterior stats:
+    posterior = Z[zmask]
+    zchain = zchain[zmask]
+
+    return posterior, zchain, zmask
+
+
+def default_parnames(npars):
+    """
+    Create an array of parameter names with sequential indices.
+
+    Parameters
+    ----------
+    npars: Integer
+        Number of parameters.
+
+    Results
+    -------
+    1D string ndarray of parameter names.
+    """
+    namelen = len(str(npars))+1
+    return np.array([f'param{i+1:0{namelen}d}' for i in range(npars)])
+
+
+def tex_parameters(
+        values, low_bounds, high_bounds, names=None, significant_digits=2,
     ):
-        # Logging object:
-        if isinstance(log, str):
-            self.log = mu.Log(log, append=resume)
-            self._closelog = True
+    r"""
+    Parse parameter values and +/- confidence intervals as LaTex strings
+    with desired number of significant digits.
+
+    Parameters
+    ----------
+    values: 1D iterable of floats
+        Parameter estimate values (e.g., best fits or posterior medians).
+        If a value is None or NaN report the range from low to high.
+    low_bounds: 1D iterable of floats
+        Lower boundary of the parameter credible intervals.
+    high_bounds: 1D iterable of floats
+        Upper boundary of the parameter credible intervals.
+    names: 1D iterable of strings
+        If not None, prepend to each output value the parameter name
+        (including an equal sign in between).
+    significant_digits: Integer
+        How many significant digits to display.
+
+    Returns
+    -------
+    tex_values: 1D list of strings
+        String representation of the estimated values as LaTeX text.
+
+    Examples
+    --------
+    >>> import mc3.utils as mu
+    >>> values    = [9.29185155e+02, -3.25725507e+00, 8.80628658e-01]
+    >>> lo_bounds = [5.29185155e+02, -4.02435791e+00, 6.43578351e-01]
+    >>> hi_bounds = [1.43406714e+03, -2.76718364e+00, 9.87000918e-01]
+
+    >>> # Default behavior:
+    >>> tex_vals = mu.tex_parameters(values, lo_bounds, hi_bounds)
+    >>> for tex in tex_vals:
+    >>>     print(tex)
+    $929.2^{+504.9}_{-400.0}$
+    $-3.26^{+0.49}_{-0.77}$
+    $0.88^{+0.11}_{-0.24}$
+
+    >>> # Custom significant digits:
+    >>> tex_vals = mu.tex_parameters(
+    >>>     values, lo_bounds, hi_bounds, significant_digits=1,
+    >>> )
+    >>> for tex in tex_vals:
+    >>>     print(tex)
+    $929.2^{+504.9}_{-400.0}$
+    $-3.3^{+0.5}_{-0.8}$
+    $0.9^{+0.1}_{-0.2}$
+
+    >>> # Including the name of the parameters:
+    >>> names = [
+    >>>     r'$T_{\rm iso}$', r'$\log\,X_{\rm H2O}$', r'$\phi_{\rm patchy}$',
+    >>> ]
+    >>> tex_vals = mu.tex_parameters(
+    >>>     values, lo_bounds, hi_bounds, names,
+    >>> )
+    >>> for tex in tex_vals:
+    >>>     print(tex)
+    $T_{\rm iso} = 929.2^{+504.9}_{-400.0}$
+    $\log\,X_{\rm H2O} = -3.26^{+0.49}_{-0.77}$
+    $\phi_{\rm patchy} = 0.88^{+0.11}_{-0.24}$
+    """
+    npars = len(values)
+    tex_values = []
+    for k in range(npars):
+        value = values[k]
+        if value is None or np.isnan(value):
+            low = low_bounds[k]
+            high = high_bounds[k]
+            dec_place = Decimal(low-high).adjusted()
+            dec = np.clip(significant_digits - 1 - dec_place, 1, 10)
+            tex_value = f'[{low:.{dec}f}, {high:.{dec}f}]'
         else:
-            if log is None:
-                self.log = mu.Log()
-            else:
-                self.log = log
-            self._closelog = False
+            low = low_bounds[k] - value
+            high = high_bounds[k] - value
 
-        log.msg(
-           f"\n{log.sep}\n"
-            "  Multi-core Markov-chain Monte Carlo (mc3).\n"
-           f"  Version {__version__}.\n"
-           f"  Copyright (c) 2015-{date.today().year} Patricio Cubillos "
-              "and collaborators.\n"
-            "  mc3 is open-source software under the MIT license (see LICENSE).\n"
-           f"{log.sep}\n\n")
-
-        if sampler is None:
-            log.error("'sampler' is a required argument")
-        if nsamples is None and sampler in ['MRW', 'DEMC', 'snooker']:
-            log.error("'nsamples' is a required argument for MCMC runs")
-        if leastsq not in [None, 'lm', 'trf']:
-            log.error(
-                f"Invalid 'leastsq' input ({leastsq}). Must select from "
-                 "['lm', 'trf']")
-
-        # Read the model parameters:
-        params = mu.isfile(params, 'params', log, 'ascii', False, not_none=True)
-        # Unpack if necessary:
-        if np.ndim(params) > 1:
-            ninfo, ndata = np.shape(params)
-            if ninfo == 7:         # The priors
-                prior = params[4]
-                priorlow = params[5]
-                priorup = params[6]
-            if ninfo >= 4:         # The stepsize
-                pstep = params[3]
-            if ninfo >= 3:         # The boundaries
-                pmin = params[1]
-                pmax = params[2]
-            else:
-                log.error('Invalid format/shape for params input file')
-            params = params[0]     # The initial guess
-        params = np.array(params)
-
-
-        # Process data and uncertainties:
-        data = mu.isfile(data, 'data', log, 'bin', False, not_none=True)
-        if np.ndim(data) > 1:
-            data, uncert = data
-        # Make local 'uncert' a copy, to avoid overwriting:
-        if uncert is None:
-            log.error("'uncert' is a required argument")
-        uncert = np.copy(uncert)
-
-        # Process the independent parameters:
-        if indparams != []:
-            indparams = mu.isfile(indparams, 'indparams', log, 'bin', unpack=False)
-
-        if ioff:
-            plt.ioff()
-
-        resume = resume and (savefile is not None)
-        if resume:
-            log.msg(f"\n\n{log.sep}\n{log.sep}  Resuming previous MCMC run.\n\n")
-
-        # Import the model function:
-        if isinstance(func, (list, tuple, np.ndarray)):
-            if len(func) == 3:
-                sys.path.append(func[2])
+            decs_low = Decimal(low).adjusted()
+            decs_high = Decimal(high).adjusted()
+            dec_place = np.min((decs_low,decs_high))
+            dec = np.clip(significant_digits - 1 - dec_place, 1, 10)
+
+            tex_value = f'{value:>.{dec}f}'
+            tex_low = f'{low:+.{dec}f}'
+            tex_high = f'{high:+.{dec}f}'
+            tex_value += f'^{{{tex_high}}}_{{{tex_low}}}'
+            # Override if parameter is fixed:
+            if low == high:
+                tex_value = f'{value}'
+
+        # Prepend parameter name if needed, care for math-mode characters:
+        if names is not None:
+            pname = names[k].strip()
+            if pname.startswith('$') and pname.endswith('$'):
+                prefix = f'{pname[:-1]} = '
             else:
-                sys.path.append(os.getcwd())
-            fmodule = importlib.import_module(func[1])
-            func = getattr(fmodule, func[0])
-        elif not callable(func):
-            log.error(
-                "'func' must be either a callable or an iterable of strings "
-                "with the model function, file, and path names")
-
-
-        if ncpu is None and sampler in ['snooker', 'demc', 'mrw']:
-            ncpu = nchains
-        elif ncpu is None and sampler == 'dynesty':
-            ncpu = 1
-        # Cap the number of processors:
-        if ncpu >= mpr.cpu_count():
-            log.warning(
-                f"The number of requested CPUs ({ncpu}) is >= than the number "
-                f"of available CPUs ({mpr.cpu_count()}).  "
-                f"Enforced ncpu to {mpr.cpu_count()-1}.")
-            ncpu = mpr.cpu_count() - 1
-
-        nparams = len(params)
-        ndata = len(data)
-
-        # Setup array of parameter names:
-        if pnames is None and texnames is not None:
-            pnames = texnames
-        elif pnames is not None and texnames is None:
-            texnames = pnames
-        elif pnames is None and texnames is None:
-            pnames = texnames = mu.default_parnames(nparams)
-        pnames = np.asarray(pnames)
-        texnames = np.asarray(texnames)
-
-        if pmin is None:
-            pmin = np.tile(-np.inf, nparams)
-        if pmax is None:
-            pmax = np.tile( np.inf, nparams)
-        pmin = np.asarray(pmin)
-        pmax = np.asarray(pmax)
-        if (np.any(np.isinf(pmin)) or np.any(np.isinf(pmax))) \
-                and sampler=='dynesty':
-            log.error('Parameter space must be constrained by pmin and pmax')
-
-        if pstep is None:
-            pstep = 0.1 * np.abs(params)
-        pstep = np.asarray(pstep)
-
-
-        # Set prior parameter indices:
-        if prior is None or priorup is None or priorlow is None:
-            prior = priorup = priorlow = np.zeros(nparams)
-
-        # Override priors for non-free parameters:
-        priorlow[pstep<=0] = 0.0
-        priorup [pstep<=0] = 0.0
-
-        # Check that initial values lie within the boundaries:
-        if np.any(params < pmin) or np.any(params > pmax):
-            pout = ""
-            for pname, par, minp, maxp in zip(pnames, params, pmin, pmax):
-                if par < minp:
-                    pout += f"\n{pname[:11]:11s}  {minp: 12.5e} < {par: 12.5e}"
-                if par > maxp:
-                    pout += f"\n{pname[:11]:26s}  {par: 12.5e} > {maxp: 12.5e}"
-
-            log.error(
-                "Some initial-guess values are out of bounds:\n"
-                "Param name           pmin          value           pmax\n"
-                "-----------  ------------   ------------   ------------"
-                f"{pout}"
-            )
-
-        nfree = int(np.sum(pstep > 0))
-        ifree = np.where(pstep > 0)[0]  # Free parameter indices
-        ishare = np.where(pstep < 0)[0]  # Shared parameter indices
-
-        # Check output dimension:
-        model0 = func(params, *indparams)
-        if np.shape(model0) != np.shape(data):
-            log.error(
-                f"The size of the data array ({np.size(data)}) does not "
-                f"match the size of the func() output ({np.size(model0)})"
-            )
-
-
-        # Check that output path exists:
-        if savefile is not None:
-            fpath, fname = os.path.split(os.path.realpath(savefile))
-            if not os.path.exists(fpath):
-                log.warning(
-                    f"Output folder path: '{fpath}' does not exist. "
-                    "Creating new folder."
-                )
-                os.makedirs(fpath)
-
-        # At the moment, skip optimization when these dynesty inputs exist:
-        if sampler == 'dynesty' \
-                and ('loglikelihood' in kwargs or 'prior_transform' in kwargs):
-            leastsq = None
-
-        # Least-squares minimization:
-        chisq_factor = 1.0
-        if leastsq is not None:
-            fit_output = fit(
-                data, uncert, func, np.copy(params), indparams,
-                pstep, pmin, pmax, prior, priorlow, priorup, leastsq)
-            fit_bestp = fit_output['bestp']
-            log.msg(
-                f"Least-squares best-fitting parameters:\n  {fit_bestp}\n\n",
-                si=2)
-
-            # Scale data-uncertainties such that reduced chisq = 1:
-            if chisqscale:
-                chisq_factor = np.sqrt(fit_output['best_chisq']/(ndata-nfree))
-                uncert *= chisq_factor
-
-                # Re-calculate best-fitting parameters with new uncertainties:
-                fit_output = fit(
-                    data, uncert, func, np.copy(params), indparams,
-                    pstep, pmin, pmax, prior, priorlow, priorup, leastsq)
-                log.msg(
-                    "Least-squares best-fitting parameters (rescaled chisq):"
-                    f"\n  {fit_output['bestp']}\n\n",
-                    si=2)
-            params = np.copy(fit_output['bestp'])
+                prefix = f'{pname}$ = '
         else:
-            fit_output = None
-
-
-        if resume:
-            with np.load(savefile) as oldrun:
-                uncert *= float(oldrun['chisq_factor'])/chisq_factor
-                chisq_factor = float(oldrun['chisq_factor'])
-
-        # Here's where the magic happens:
-        if sampler in ['mrw', 'demc', 'snooker']:
-            output = mcmc(
-                data, uncert, func, params, indparams, pmin, pmax, pstep,
-                prior, priorlow, priorup, nchains, ncpu, nsamples, sampler,
-                wlike, fit_output, grtest, grbreak, grnmin, burnin, thinning,
-                fgamma, fepsilon, hsize, kickoff, savefile, resume, log,
-                pnames, texnames,
-            )
-        elif sampler == 'dynesty':
-            output = nested_sampling(
-                data, uncert, func, params, indparams,
-                pmin, pmax, pstep, prior, priorlow, priorup, ncpu,
-                thinning, resume, log, **kwargs,
-            )
-
-
-        # Get some stats:
-        output['pnames'] = pnames
-        output['texnames'] = texnames
-        output['chisq_factor'] = chisq_factor
-
-        if leastsq is not None:
-            delta_log_post = output['best_log_post'] - fit_output['best_log_post']
-            delta_pars = output['bestp'] - fit_output['bestp']
-            if delta_log_post > 5.0e-8 and np.any(delta_pars != 0.0):
-                log.warning(
-                    "MCMC found a better fit than the minimizer:\n"
-                    "MCMC best-fitting parameters:        (chisq={:.8g})\n{}\n"
-                    "Minimizer best-fitting parameters:   (chisq={:.8g})\n{}".
-                    format(
-                        -2*output['best_log_post'], output['bestp'],
-                        -2*fit_output['best_log_post'], fit_output['bestp']))
-
-        # And remove burn-in samples:
-        posterior, zchain, zmask = mu.burn(
-            Z=output['posterior'], zchain=output['zchain'], burnin=output['burnin'])
-
-        # TBD: make this user-configurable
-        theme = mp.THEMES['blue']
-        post = mp.Posterior(posterior, pnames=texnames[ifree], theme=theme)
-
-        # Parameter statistics:
-        bestp = output['bestp']
-        sample_stats = ms.calc_sample_statistics(
-            post.posterior, bestp, pstep, hpd=True,
-        )
-        stdp = output['stdp'] = sample_stats[3]
-        median = sample_stats[0]
-        med_low_bounds = sample_stats[4]
-        med_high_bounds = sample_stats[5]
-
-
-        log.msg(
-            "\nParameter name     best fit   median      1sigma_low   1sigma_hi        S/N"
-            "\n--------------- -----------  -----------------------------------  ---------",
-            width=80)
-        for i in range(nparams):
-            pname = f'{pnames[i][0:15]:<15}'
-            lo = med_low_bounds[i] - median[i]
-            hi = med_high_bounds[i] - median[i]
-            if i in ifree:
-                snr = f"{np.abs(bestp[i])/stdp[i]:.1f}"
-            elif i in ishare:
-                idx = -int(pstep[i])
-                snr = f"[share{idx:02d}]"
-            else:
-                snr = "[fixed]"
-                lo = hi = 0.0
-            log.msg(
-                f"{pname} {bestp[i]:11.4e}  {median[i]:11.4e} "
-                f"{lo:11.4e} {hi:11.4e}  {snr:>9s}",
-                width=160,
-            )
-
-        # Fit statistics:
-        best_chisq = output['best_chisq']
-        log_post = -2.0*output['best_log_post']
-        bic = output['BIC']
-        red_chisq = output['red_chisq']
-        std_dev = output['stddev_residuals']
-
-        chisqscale_txt = f"sqrt(reduced chi-squared) factor: {chisq_factor:.4f}\n"
-        if not chisqscale:
-            chisqscale_txt = ''
-
-
-        fmt = len(f"{bic:.4f}")  # Length of string formatting
-        log.msg(
-            f"\n{chisqscale_txt}"
-            f"Best-parameter's chi-squared:       {best_chisq:{fmt}.4f}\n"
-            f"Best-parameter's -2*log(posterior): {log_post:{fmt}.4f}\n"
-            f"Bayesian Information Criterion:     {bic:{fmt}.4f}\n"
-            f"Reduced chi-squared:                {red_chisq:{fmt}.4f}\n"
-            f"Standard deviation of residuals:  {std_dev:.6g}\n",
-            indent=2,
-        )
-
-        if savefile is not None or plots or closelog:
-            log.msg("\nOutput sampler files:")
+            prefix = '$'
+        tex_value = f'{prefix}{tex_value}$'
 
-        # Save results (pop unpickables before saving, then put back):
-        if savefile is not None:
-            unpickables = ['dynesty_sampler']
-            unpickables = np.intersect1d(unpickables, list(output.keys()))
-            tmp_outputs = {key: output.pop(key) for key in unpickables}
-            np.savez(savefile, **output)
-            output.update(tmp_outputs)
-            log.msg(f"'{savefile}'", indent=2)
-
-
-        if plots:
-            # Extract filename from savefile or default to sampler:
-            fname = sampler if savefile is None else os.path.splitext(savefile)[0]
-            # Include bestp in posterior plots:
-            best_freepars = output['bestp'][ifree] if showbp else None
-
-            bestp = best_freepars
-            # Trace plot:
-            savefile = f'{fname}_trace.png'
-            mp.trace(
-                output['posterior'], zchain=output['zchain'],
-                burnin=output['burnin'], pnames=texnames[ifree],
-                savefile=savefile, color=theme.color,
-            )
-            log.msg(savefile, indent=2)
-            # Pairwise posteriors:
-            savefile = f'{fname}_pairwise_posterior.png'
-            post.plot(savefile=savefile)
-            log.msg(savefile, indent=2)
-            # Histograms:
-            savefile = f'{fname}_marginal_posterior.png'
-            post.plot_histogram(savefile=savefile)
-            log.msg(savefile, indent=2)
-            # RMS vs bin size:
-            if rms:
-                savefile = f'{fname}_RMS.png'
-                residuals = output['best_model'] - data
-                data_rms, rms_lo, rms_hi, stderr, binsize = ms.time_avg(residuals)
-                mp.rms(
-                    binsize, data_rms, stderr, rms_lo, rms_hi,
-                    binstep=len(binsize)//500+1,
-                    savefile=savefile,
-                )
-                log.msg(savefile, indent=2)
-            # Guessing that indparams[0] is the X array for data as in y=y(x):
-            if (indparams != []
-                    and isinstance(indparams[0], (list, tuple, np.ndarray))
-                    and np.size(indparams[0]) == ndata):
-                try:
-                    mp.modelfit(
-                        data, uncert, indparams[0], output['best_model'],
-                        savefile=fname+"_model.png")
-                    log.msg(f"'{fname}_model.png'", indent=2)
-                except:
-                    pass
-
-        # Close the log file if necessary:
-        if closelog:
-            log.msg(f"'{log.logname}'", indent=2)
-            log.close()
+        tex_values.append(tex_value)
 
-        return output
+    return tex_values
```

### Comparing `mc3-3.1.2/mc3/sampler_driver.py` & `mc3-3.1.3/mc3/sampler_driver.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3/stats/__init__.py` & `mc3-3.1.3/mc3/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3/stats/gelman.py` & `mc3-3.1.3/mc3/stats/gelman.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3/stats/prayer.py` & `mc3-3.1.3/mc3/stats/prayer.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3/stats/stats.py` & `mc3-3.1.3/mc3/stats/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -463,15 +463,15 @@
     # Indices of the highest posterior density:
     iHPD = np.where(cdf >= quantile*cdf[-1])[0][0]
     # Minimum density in the HPD region:
     HPDmin = np.amin(pdf[ip][0:iHPD])
     return pdf, xpdf, HPDmin
 
 
-class ppf_uniform(object):
+class ppf_uniform():
     """
     Percent-point function (PPF) for a uniform function between
     pmin and pmax.  Also known as inverse CDF or quantile function.
 
     Parameters
     ----------
     pmin: Float
@@ -500,65 +500,83 @@
         self.pmin = pmin
         self.pmax = pmax
 
     def __call__(self, u):
         return (self.pmax-self.pmin)*u + self.pmin
 
 
-class ppf_gaussian(object):
+class ppf_gaussian():
     """
-    Percent-point function (PPF) for a two-sided Gaussian function
+    Percent-point function (PPF) for a Gaussian distribution
+    (with potentially assymetric standard deviations)
     Also known as inverse CDF or quantile function.
 
     Parameters
     ----------
     loc: Float
         Center of the Gaussian function.
-    lo: Float
+    sigma_lo: Float
         Left-sided standard deviation (for values x < loc).
-    up: Float
+    sigma_up: Float
         Right-sided standard deviation (for values x > loc).
-
-    Returns
-    -------
-    ppf: Callable
-        The Gaussian's PPF.
+    pmin: Float
+        Left-sided domain boundary of the PPF.
+    pmax: Float
+        Right-sided domain boundary of the PPF.
 
     Examples
     --------
     >>> import mc3.stats as ms
-    >>> ppf_g = ms.ppf_gaussian(0.0, 1.0, 1.0)
+    >>> ppf_g = ms.ppf_gaussian(2.0, 1.0, 1.0)
     >>> # The domain of the output function is (0,1):
-    >>> print(ppf_g(1e-10), ppf_g(0.5), ppf_g(1.0-1e-10))
-    (-6.361340902404056, 0.0, 6.361340889697422)
+    >>> print(ppf_g(0.5))
+    2.0
+
+    >>> print(ppf_g(0.158))
+    0.9972883349734507
+
     >>> # Also works for np.array inputs:
-    >>> print(ppf_g(np.array([1e-10, 0.5, 1-1e-10])))
-    [-6.3613409   0.          6.36134089]
+    >>> print(ppf_g(np.array([0.025, 0.158, 0.5, 0.6])))
+    [0.04003602 0.99728833 2.         2.2533471 ]
     """
-    def __init__(self, loc, lo, up):
+    def __init__(self, loc, sigma_lo, sigma_up, pmin=-np.inf, pmax=np.inf):
         self.loc = loc
-        self.lo = lo
-        self.up = up
+        self.sigma_lo = sigma_lo
+        self.sigma_up = sigma_up
+        self.pmin = pmin
+        self.pmax = pmax
+        a = (self.pmin - self.loc) / self.sigma_lo
+        b = (self.pmax - self.loc) / self.sigma_up
+        self.rv_lo = ss.truncnorm(a, b, loc=loc, scale=sigma_lo)
+        if sigma_up != sigma_lo:
+            self.rv_up = ss.truncnorm(a, b, loc=loc, scale=sigma_up)
+        self.u_threshold = sigma_lo/(sigma_lo+sigma_up)
+        self._ufactor1 = 1.0 + sigma_up/sigma_lo
+        self._ufactor2 = 1.0 + sigma_lo/sigma_up
 
     def __call__(self, u):
-        if np.isscalar(u) and u < self.lo/(self.lo+self.up):
-            return ss.norm.ppf(0.5*u*(self.lo+self.up)/self.lo,
-                scale=self.lo, loc=self.loc)
-        elif np.isscalar(u):
-            return ss.norm.ppf(1-0.5*(1-u)*(1+self.lo/self.up),
-                scale=self.up, loc=self.loc)
-        # else:
+        if self.sigma_lo == self.sigma_up:
+            return self.rv_lo.ppf(u)
+
+        if np.isscalar(u):
+            if u < self.u_threshold:
+                return self.rv_lo.ppf(0.5*u*self._ufactor1)
+            return self.rv_up.ppf(1.0-0.5*(1-u)*self._ufactor2)
+
         icdf = np.empty_like(u)
-        left = u < self.lo/(self.lo+self.up)
-        icdf[ left] = ss.norm.ppf(0.5*u[left]*(1+self.up/self.lo),
-            scale=self.lo, loc=self.loc)
-        icdf[~left] = ss.norm.ppf(1-0.5*(1-u[~left])*(1+self.lo/self.up),
-            scale=self.up, loc=self.loc)
+        left = u < self.u_threshold
+        icdf[left] = self.rv_lo.ppf(0.5*u[left]*self._ufactor1)
+        icdf[~left] = self.rv_up.ppf(1.0-0.5*(1-u[~left])*self._ufactor2)
         return icdf
 
+    def draw(self, size):
+        u = np.random.uniform(size=size)
+        samples = self.__call__(u)
+        return samples
+
 
 def dwt_daub4(array, inverse=False):
     """
     1D discrete wavelet transform using the Daubechies 4-parameter wavelet
 
     Parameters
     ----------
@@ -597,48 +615,55 @@
     """
     Wrapper to compute log(likelihood)
 
     If there's any non-finite value in the model function
     (sign of an invalid parameter set), return a large-negative
     log likelihood (to reject the sample).
     """
-    def __init__(self, data, uncert, func, params, indp, pstep):
+    def __init__(self, data, uncert, func, params, args, pstep):
         self.data = data
         self.uncert = uncert
         self.func = func
         self.params = params
-        self.indp = indp
+        self.args = args
         self.pstep = pstep
         self.ifree = pstep>0
         self.ishare = np.where(pstep<0)[0]
+
+        # Pre-calculate the part outside chi-square:
+        self._uncert_logl = -0.5*np.sum(np.log(2.0*np.pi*self.uncert**2.0))
+
+
     def __call__(self, params):
         self.params[self.ifree] = params
         for s in self.ishare:
             self.params[s] = self.params[-int(self.pstep[s])-1]
-        model = self.func(self.params, *self.indp)
+
+        model = self.func(self.params, *self.args)
         log_like = -0.5 * np.sum(
             ((self.data - model) / self.uncert)**2.0
         )
+        log_like += self._uncert_logl
         if not np.isfinite(log_like):
             log_like = -1.0e98
         return log_like
 
 
-class Prior_transform(object):
+class Prior_transform():
     """Wrapper to compute the PPF of a set of parameters."""
     def __init__(self, prior, priorlow, priorup, pmin, pmax, pstep):
         self.ppf = []
         for p0, plo, pup, min, max, step in \
             zip(prior, priorlow, priorup, pmin, pmax, pstep):
             if step <= 0:
                 continue
             if plo == 0.0 or pup == 0.0:
                 self.ppf.append(ppf_uniform(min, max))
             else:
-                self.ppf.append(ppf_gaussian(p0, plo, pup))
+                self.ppf.append(ppf_gaussian(p0, plo, pup, min, max))
     def __call__(self, u):
         return [ppf(v) for ppf,v in zip(self.ppf, u)]
 
 
 def marginal_statistics(
         posterior, statistics='med_central', quantile=0.683,
         pdf=None, xpdf=None,
```

### Comparing `mc3-3.1.2/mc3/stats/time_averaging.py` & `mc3-3.1.3/mc3/stats/time_averaging.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3/utils/__init__.py` & `mc3-3.1.3/mc3/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3/utils/log.py` & `mc3-3.1.3/mc3/utils/log.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/mc3.egg-info/PKG-INFO` & `mc3-3.1.3/mc3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mc3
-Version: 3.1.2
+Version: 3.1.3
 Summary: Multi-core Markov-chain Monte Carlo package.
 Home-page: https://github.com/pcubillos/mc3
 Author: Patricio Cubillos
 Author-email: patricio.cubillos@oeaw.ac.at
 License: MIT
 Description: # mc3: Multi-core Markov-chain Monte Carlo
         > A Python implementation of the Markov-chain Monte Carlo algorithm.
```

### Comparing `mc3-3.1.2/mc3.egg-info/SOURCES.txt` & `mc3-3.1.3/mc3.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,33 +24,34 @@
 docs/figures/quad_fitting.png
 docs/figures/quad_hist.png
 docs/figures/quad_pairwise.png
 docs/figures/quad_trace.png
 docs/figures/rms-vs-binsize.png
 examples/get_started.py
 examples/ns_tutorial.py
+examples/ppf.py
 examples/timeavg.py
 examples/tutorial.py
 mc3/__init__.py
 mc3/__main__.py
 mc3/chain.py
 mc3/fit_driver.py
 mc3/mcmc_driver.py
 mc3/ns_driver.py
-mc3/sampler.py
 mc3/sampler_driver.py
 mc3/version.py
 mc3.egg-info/PKG-INFO
 mc3.egg-info/SOURCES.txt
 mc3.egg-info/dependency_links.txt
 mc3.egg-info/entry_points.txt
 mc3.egg-info/requires.txt
 mc3.egg-info/top_level.txt
 mc3/plots/__init__.py
 mc3/plots/colors.py
+mc3/plots/mc3_plots.py
 mc3/plots/plot_functions.py
 mc3/plots/posterior.py
 mc3/stats/__init__.py
 mc3/stats/gelman.py
 mc3/stats/prayer.py
 mc3/stats/stats.py
 mc3/stats/time_averaging.py
```

### Comparing `mc3-3.1.2/setup.py` & `mc3-3.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 incdir = 'src_c/include/'
 
 cfiles = os.listdir(srcdir)
 cfiles = list(filter(lambda x: re.search('.+[.]c$', x), cfiles))
 cfiles = list(filter(lambda x: not re.search('[.#].+[.]c$', x), cfiles))
 
 inc = [get_include(), incdir]
-eca = ['-ffast-math']
+eca = ['-O3', '-ffast-math']
 ela = []
 
 extensions = [
     Extension(
         'mc3.lib.' + cfile.rstrip('.c'),
         sources=[f'{srcdir}{cfile}'],
         include_dirs=inc,
```

### Comparing `mc3-3.1.2/src_c/_binarray.c` & `mc3-3.1.3/src_c/_binarray.c`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/src_c/_chisq.c` & `mc3-3.1.3/src_c/_chisq.c`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/src_c/_dwt.c` & `mc3-3.1.3/src_c/_dwt.c`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/src_c/_time_averaging.c` & `mc3-3.1.3/src_c/_time_averaging.c`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/src_c/include/ind.h` & `mc3-3.1.3/src_c/include/ind.h`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/src_c/include/stats.h` & `mc3-3.1.3/src_c/include/stats.h`

 * *Files 1% similar despite different names*

```diff
@@ -32,20 +32,20 @@
 n: Number of values to calculate the mean.
 
 Returns
 -------
 datarms: The root mean square of the data.
 ******************************************************************/
 double rms(double *data, const int n){
-  int i;
-  double datarms=0.0;
-  for (i=0; i<n; i++)
-    datarms += data[i]*data[i];
-  datarms = sqrt(datarms/n);
-  return datarms;
+    int i;
+    double datarms=0.0;
+    for (i=0; i<n; i++)
+        datarms += data[i]*data[i];
+    datarms = sqrt(datarms/n);
+    return datarms;
 }
 
 
 /******************************************************************
 Calculate the standard deviation of the first n elements of data.
 
 Parameters
```

### Comparing `mc3-3.1.2/src_c/include/wavelet.h` & `mc3-3.1.3/src_c/include/wavelet.h`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/tests/test_dynesty.py` & `mc3-3.1.3/tests/test_dynesty.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/tests/test_fit.py` & `mc3-3.1.3/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/tests/test_logging.py` & `mc3-3.1.3/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/tests/test_mcmc.py` & `mc3-3.1.3/tests/test_mcmc.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/tests/test_plots.py` & `mc3-3.1.3/tests/test_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,18 +106,18 @@
 
 
 def test_Theme():
     color = 'xkcd:blue'
     theme = mp.Theme(color)
 
     expected_light_color = np.array([0.25882353, 0.44705882, 0.90588235])
-    expected_dark_color = np.array([0.00588235, 0.13137255, 0.4372549 ])
+    expected_dark_color = np.array([0.00823529, 0.18392157, 0.61215686])
     expected_bad = expected_under = np.array([1., 1., 1., 1.])
     expected_first = np.array([0.85176471, 0.88941176, 0.98117647])
-    expected_last = np.array([0.00588235, 0.13137255, 0.4372549 ])
+    expected_last = np.array([0.00823529, 0.18392157, 0.61215686])
 
     assert theme.color == color
     np.testing.assert_allclose(theme.light_color, expected_light_color, rtol)
     np.testing.assert_allclose(theme.dark_color, expected_dark_color, rtol)
 
     colormap = theme.colormap
     assert colormap.N == 256
```

### Comparing `mc3-3.1.2/tests/test_stats.py` & `mc3-3.1.3/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.2/tests/test_utils.py` & `mc3-3.1.3/tests/test_utils.py`

 * *Files identical despite different names*

