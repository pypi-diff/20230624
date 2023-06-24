# Comparing `tmp/cocotbext-pcie-0.2.6.tar.gz` & `tmp/cocotbext-pcie-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocotbext-pcie-0.2.6.tar", last modified: Thu Jul  7 06:10:27 2022, max compression
+gzip compressed data, was "cocotbext-pcie-0.2.8.tar", last modified: Wed Jul 13 06:38:07 2022, max compression
```

## Comparing `cocotbext-pcie-0.2.6.tar` & `cocotbext-pcie-0.2.8.tar`

### file list

```diff
@@ -1,72 +1,80 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.192474 cocotbext-pcie-0.2.6/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.179138 cocotbext-pcie-0.2.6/.github/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.182472 cocotbext-pcie-0.2.6/.github/workflows/
--rw-r--r--   0 alex      (1000) alex      (1000)      816 2022-03-16 04:41:12.000000 cocotbext-pcie-0.2.6/.github/workflows/regression-tests.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      138 2020-12-11 02:49:56.000000 cocotbext-pcie-0.2.6/.gitignore
--rw-r--r--   0 alex      (1000) alex      (1000)     1059 2020-12-11 02:49:56.000000 cocotbext-pcie-0.2.6/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)       86 2020-12-11 02:49:56.000000 cocotbext-pcie-0.2.6/MANIFEST.in
--rw-r--r--   0 alex      (1000) alex      (1000)     4071 2022-07-07 06:10:27.192474 cocotbext-pcie-0.2.6/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     3147 2021-11-03 05:16:53.000000 cocotbext-pcie-0.2.6/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.179138 cocotbext-pcie-0.2.6/cocotbext/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.182472 cocotbext-pcie-0.2.6/cocotbext/pcie/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.185806 cocotbext-pcie-0.2.6/cocotbext/pcie/core/
--rw-r--r--   0 alex      (1000) alex      (1000)     1262 2020-12-11 02:49:56.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)    24088 2022-03-16 04:41:12.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/bridge.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.185806 cocotbext-pcie-0.2.6/cocotbext/pcie/core/caps/
--rw-r--r--   0 alex      (1000) alex      (1000)     1348 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/caps/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)    23027 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/caps/aer.py
--rw-r--r--   0 alex      (1000) alex      (1000)     7992 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/caps/common.py
--rw-r--r--   0 alex      (1000) alex      (1000)    11455 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/caps/msi.py
--rw-r--r--   0 alex      (1000) alex      (1000)    32935 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/caps/pcie.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3957 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/caps/pm.py
--rw-r--r--   0 alex      (1000) alex      (1000)     6028 2021-11-17 08:50:11.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/device.py
--rw-r--r--   0 alex      (1000) alex      (1000)     8164 2021-04-29 03:31:27.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/dllp.py
--rw-r--r--   0 alex      (1000) alex      (1000)    16844 2021-11-17 08:50:11.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/endpoint.py
--rw-r--r--   0 alex      (1000) alex      (1000)    28754 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/function.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2376 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/msi.py
--rw-r--r--   0 alex      (1000) alex      (1000)    43321 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/pci.py
--rw-r--r--   0 alex      (1000) alex      (1000)    26870 2022-03-16 04:41:12.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/port.py
--rw-r--r--   0 alex      (1000) alex      (1000)    35212 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/rc.py
--rw-r--r--   0 alex      (1000) alex      (1000)     7231 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/region.py
--rw-r--r--   0 alex      (1000) alex      (1000)     8611 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/switch.py
--rw-r--r--   0 alex      (1000) alex      (1000)    24456 2021-11-17 08:50:11.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/tlp.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2553 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/utils.py
--rw-r--r--   0 alex      (1000) alex      (1000)       22 2022-07-07 06:10:25.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/core/version.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.182472 cocotbext-pcie-0.2.6/cocotbext/pcie/intel/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.189140 cocotbext-pcie-0.2.6/cocotbext/pcie/intel/s10/
--rw-r--r--   0 alex      (1000) alex      (1000)     1164 2021-11-03 05:16:53.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/intel/s10/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)    20682 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/intel/s10/interface.py
--rw-r--r--   0 alex      (1000) alex      (1000)    41961 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/intel/s10/s10_model.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.182472 cocotbext-pcie-0.2.6/cocotbext/pcie/xilinx/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.189140 cocotbext-pcie-0.2.6/cocotbext/pcie/xilinx/us/
--rw-r--r--   0 alex      (1000) alex      (1000)     1211 2020-12-11 02:49:56.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/xilinx/us/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)    40472 2022-07-07 06:10:25.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/xilinx/us/interface.py
--rw-r--r--   0 alex      (1000) alex      (1000)    20649 2021-11-17 08:50:11.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/xilinx/us/tlp.py
--rw-r--r--   0 alex      (1000) alex      (1000)    63730 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/xilinx/us/us_model.py
--rw-r--r--   0 alex      (1000) alex      (1000)    68423 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.6/cocotbext/pcie/xilinx/us/usp_model.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.189140 cocotbext-pcie-0.2.6/cocotbext_pcie.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     4071 2022-07-07 06:10:26.000000 cocotbext-pcie-0.2.6/cocotbext_pcie.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     1559 2022-07-07 06:10:27.000000 cocotbext-pcie-0.2.6/cocotbext_pcie.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2022-07-07 06:10:26.000000 cocotbext-pcie-0.2.6/cocotbext_pcie.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       63 2022-07-07 06:10:26.000000 cocotbext-pcie-0.2.6/cocotbext_pcie.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       10 2022-07-07 06:10:27.000000 cocotbext-pcie-0.2.6/cocotbext_pcie.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)     1792 2022-07-07 06:10:27.192474 cocotbext-pcie-0.2.6/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)       37 2020-12-11 02:49:56.000000 cocotbext-pcie-0.2.6/setup.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.189140 cocotbext-pcie-0.2.6/tests/
--rw-r--r--   0 alex      (1000) alex      (1000)     1250 2020-12-11 02:49:56.000000 cocotbext-pcie-0.2.6/tests/Makefile
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.189140 cocotbext-pcie-0.2.6/tests/pcie/
--rw-r--r--   0 alex      (1000) alex      (1000)     1345 2021-03-07 03:03:05.000000 cocotbext-pcie-0.2.6/tests/pcie/Makefile
--rw-r--r--   0 alex      (1000) alex      (1000)    23380 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.6/tests/pcie/test_pcie.py
--rw-r--r--   0 alex      (1000) alex      (1000)       97 2021-11-03 05:16:53.000000 cocotbext-pcie-0.2.6/tests/pcie/test_pcie.v
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.192474 cocotbext-pcie-0.2.6/tests/pcie_s10/
--rw-r--r--   0 alex      (1000) alex      (1000)     2691 2021-11-03 05:16:53.000000 cocotbext-pcie-0.2.6/tests/pcie_s10/Makefile
--rw-r--r--   0 alex      (1000) alex      (1000)    31980 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.6/tests/pcie_s10/test_pcie_s10.py
--rw-r--r--   0 alex      (1000) alex      (1000)     7618 2021-11-03 05:16:53.000000 cocotbext-pcie-0.2.6/tests/pcie_s10/test_pcie_s10.v
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.192474 cocotbext-pcie-0.2.6/tests/pcie_us/
--rw-r--r--   0 alex      (1000) alex      (1000)     2957 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.6/tests/pcie_us/Makefile
--rw-r--r--   0 alex      (1000) alex      (1000)    34599 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.6/tests/pcie_us/test_pcie_us.py
--rw-r--r--   0 alex      (1000) alex      (1000)     9198 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.6/tests/pcie_us/test_pcie_us.v
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-07 06:10:27.192474 cocotbext-pcie-0.2.6/tests/pcie_usp/
--rw-r--r--   0 alex      (1000) alex      (1000)     3153 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.6/tests/pcie_usp/Makefile
--rw-r--r--   0 alex      (1000) alex      (1000)    36121 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.6/tests/pcie_usp/test_pcie_usp.py
--rw-r--r--   0 alex      (1000) alex      (1000)     9057 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.6/tests/pcie_usp/test_pcie_usp.v
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.301015 cocotbext-pcie-0.2.8/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.287679 cocotbext-pcie-0.2.8/.github/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.287679 cocotbext-pcie-0.2.8/.github/workflows/
+-rw-r--r--   0 alex      (1000) alex      (1000)      816 2022-03-16 04:41:12.000000 cocotbext-pcie-0.2.8/.github/workflows/regression-tests.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      138 2020-12-11 02:49:56.000000 cocotbext-pcie-0.2.8/.gitignore
+-rw-r--r--   0 alex      (1000) alex      (1000)     1059 2020-12-11 02:49:56.000000 cocotbext-pcie-0.2.8/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)       86 2020-12-11 02:49:56.000000 cocotbext-pcie-0.2.8/MANIFEST.in
+-rw-r--r--   0 alex      (1000) alex      (1000)     4442 2022-07-13 06:38:07.301015 cocotbext-pcie-0.2.8/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     3518 2022-07-13 06:38:06.000000 cocotbext-pcie-0.2.8/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.287679 cocotbext-pcie-0.2.8/cocotbext/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.287679 cocotbext-pcie-0.2.8/cocotbext/pcie/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.291013 cocotbext-pcie-0.2.8/cocotbext/pcie/core/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1262 2020-12-11 02:49:56.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    24088 2022-03-16 04:41:12.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/bridge.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.294347 cocotbext-pcie-0.2.8/cocotbext/pcie/core/caps/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1348 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/caps/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    23027 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/caps/aer.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     7992 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/caps/common.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    11455 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/caps/msi.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    32935 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/caps/pcie.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3957 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/caps/pm.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6028 2021-11-17 08:50:11.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/device.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     8164 2021-04-29 03:31:27.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/dllp.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    16844 2021-11-17 08:50:11.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/endpoint.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    28754 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/function.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2376 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/msi.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    43321 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/pci.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    26870 2022-03-16 04:41:12.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/port.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    35212 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/rc.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     7231 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/region.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     8611 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/switch.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    24456 2021-11-17 08:50:11.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/tlp.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2553 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/utils.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       22 2022-07-13 06:38:06.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/core/version.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.287679 cocotbext-pcie-0.2.8/cocotbext/pcie/intel/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.294347 cocotbext-pcie-0.2.8/cocotbext/pcie/intel/ptile/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1174 2022-07-13 06:38:06.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/intel/ptile/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    22965 2022-07-13 06:38:06.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/intel/ptile/interface.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    48563 2022-07-13 06:38:06.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/intel/ptile/ptile_model.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.294347 cocotbext-pcie-0.2.8/cocotbext/pcie/intel/s10/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1164 2021-11-03 05:16:53.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/intel/s10/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    20682 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/intel/s10/interface.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    41961 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/intel/s10/s10_model.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.287679 cocotbext-pcie-0.2.8/cocotbext/pcie/xilinx/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.294347 cocotbext-pcie-0.2.8/cocotbext/pcie/xilinx/us/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1211 2020-12-11 02:49:56.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/xilinx/us/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    40472 2022-07-07 06:10:25.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/xilinx/us/interface.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    20649 2021-11-17 08:50:11.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/xilinx/us/tlp.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    63730 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/xilinx/us/us_model.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    68423 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.8/cocotbext/pcie/xilinx/us/usp_model.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.297681 cocotbext-pcie-0.2.8/cocotbext_pcie.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     4442 2022-07-13 06:38:06.000000 cocotbext-pcie-0.2.8/cocotbext_pcie.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     1777 2022-07-13 06:38:07.000000 cocotbext-pcie-0.2.8/cocotbext_pcie.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2022-07-13 06:38:06.000000 cocotbext-pcie-0.2.8/cocotbext_pcie.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       63 2022-07-13 06:38:07.000000 cocotbext-pcie-0.2.8/cocotbext_pcie.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       10 2022-07-13 06:38:07.000000 cocotbext-pcie-0.2.8/cocotbext_pcie.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)     1792 2022-07-13 06:38:07.301015 cocotbext-pcie-0.2.8/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)       37 2020-12-11 02:49:56.000000 cocotbext-pcie-0.2.8/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.297681 cocotbext-pcie-0.2.8/tests/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1250 2020-12-11 02:49:56.000000 cocotbext-pcie-0.2.8/tests/Makefile
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.297681 cocotbext-pcie-0.2.8/tests/pcie/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1345 2021-03-07 03:03:05.000000 cocotbext-pcie-0.2.8/tests/pcie/Makefile
+-rw-r--r--   0 alex      (1000) alex      (1000)    23380 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.8/tests/pcie/test_pcie.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       97 2021-11-03 05:16:53.000000 cocotbext-pcie-0.2.8/tests/pcie/test_pcie.v
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.297681 cocotbext-pcie-0.2.8/tests/pcie_ptile/
+-rw-r--r--   0 alex      (1000) alex      (1000)     3465 2022-07-13 06:38:06.000000 cocotbext-pcie-0.2.8/tests/pcie_ptile/Makefile
+-rw-r--r--   0 alex      (1000) alex      (1000)    36598 2022-07-13 06:38:06.000000 cocotbext-pcie-0.2.8/tests/pcie_ptile/test_pcie_ptile.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    11959 2022-07-13 06:38:06.000000 cocotbext-pcie-0.2.8/tests/pcie_ptile/test_pcie_ptile.v
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.297681 cocotbext-pcie-0.2.8/tests/pcie_s10/
+-rw-r--r--   0 alex      (1000) alex      (1000)     2691 2021-11-03 05:16:53.000000 cocotbext-pcie-0.2.8/tests/pcie_s10/Makefile
+-rw-r--r--   0 alex      (1000) alex      (1000)    31980 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.8/tests/pcie_s10/test_pcie_s10.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     7618 2021-11-03 05:16:53.000000 cocotbext-pcie-0.2.8/tests/pcie_s10/test_pcie_s10.v
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.297681 cocotbext-pcie-0.2.8/tests/pcie_us/
+-rw-r--r--   0 alex      (1000) alex      (1000)     2957 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.8/tests/pcie_us/Makefile
+-rw-r--r--   0 alex      (1000) alex      (1000)    34599 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.8/tests/pcie_us/test_pcie_us.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     9198 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.8/tests/pcie_us/test_pcie_us.v
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2022-07-13 06:38:07.301015 cocotbext-pcie-0.2.8/tests/pcie_usp/
+-rw-r--r--   0 alex      (1000) alex      (1000)     3153 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.8/tests/pcie_usp/Makefile
+-rw-r--r--   0 alex      (1000) alex      (1000)    36121 2022-06-05 07:15:32.000000 cocotbext-pcie-0.2.8/tests/pcie_usp/test_pcie_usp.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     9057 2022-05-30 00:22:23.000000 cocotbext-pcie-0.2.8/tests/pcie_usp/test_pcie_usp.v
```

### Comparing `cocotbext-pcie-0.2.6/.github/workflows/regression-tests.yml` & `cocotbext-pcie-0.2.8/.github/workflows/regression-tests.yml`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/LICENSE` & `cocotbext-pcie-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/PKG-INFO` & `cocotbext-pcie-0.2.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocotbext-pcie
-Version: 0.2.6
+Version: 0.2.8
 Summary: PCI express simulation framework for cocotb
 Home-page: https://github.com/alexforencich/cocotbext-pcie
 Download-URL: https://github.com/alexforencich/cocotbext-pcie/tarball/master
 Author: Alex Forencich
 Author-email: alex@alexforencich.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/alexforencich/cocotbext-pcie/issues
@@ -64,8 +64,12 @@
 
 Models of the Xilinx UltraScale and UltraScale+ PCIe hard cores are included in `cocotbext.pcie.xilinx.us`.  These modules can be used in combination with the PCIe BFM to test an HDL design that targets Xilinx UltraScale, UltraScale+, or Virtex 7 series FPGAs, up to PCIe gen 3 x16 or PCIe gen 4 x8.  The models currently only support operation as a device, not as a root port.
 
 #### Intel Stratix 10 H-Tile/L-Tile
 
 Models of the Intel Stratix 10 H-Tile/L-Tile PCIe hard cores are included in `cocotbext.pcie.intel.s10`.  These modules can be used in combination with the PCIe BFM to test an HDL design that targets Intel Stratix 10 GX, SX, TX, and MX series FPGAs that contain H-Tiles or L-Tiles, up to PCIe gen 3 x16.  The models currently only support operation as a device, not as a root port.
 
+#### Intel P-Tile
+
+Models of the Intel P-Tile PCIe hard cores are included in `cocotbext.pcie.intel.ptile`.  These modules can be used in combination with the PCIe BFM to test an HDL design that targets Intel Stratix 10 DX or Agilex F series FPGAs that contain P-Tiles, up to PCIe gen 4 x16.  The models currently only support operation as a device, not as a root port.
+
```

### Comparing `cocotbext-pcie-0.2.6/README.md` & `cocotbext-pcie-0.2.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -39,7 +39,11 @@
 #### Xilinx UltraScale and UltraScale+
 
 Models of the Xilinx UltraScale and UltraScale+ PCIe hard cores are included in `cocotbext.pcie.xilinx.us`.  These modules can be used in combination with the PCIe BFM to test an HDL design that targets Xilinx UltraScale, UltraScale+, or Virtex 7 series FPGAs, up to PCIe gen 3 x16 or PCIe gen 4 x8.  The models currently only support operation as a device, not as a root port.
 
 #### Intel Stratix 10 H-Tile/L-Tile
 
 Models of the Intel Stratix 10 H-Tile/L-Tile PCIe hard cores are included in `cocotbext.pcie.intel.s10`.  These modules can be used in combination with the PCIe BFM to test an HDL design that targets Intel Stratix 10 GX, SX, TX, and MX series FPGAs that contain H-Tiles or L-Tiles, up to PCIe gen 3 x16.  The models currently only support operation as a device, not as a root port.
+
+#### Intel P-Tile
+
+Models of the Intel P-Tile PCIe hard cores are included in `cocotbext.pcie.intel.ptile`.  These modules can be used in combination with the PCIe BFM to test an HDL design that targets Intel Stratix 10 DX or Agilex F series FPGAs that contain P-Tiles, up to PCIe gen 4 x16.  The models currently only support operation as a device, not as a root port.
```

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/__init__.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/bridge.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/bridge.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/caps/__init__.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/caps/__init__.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/caps/aer.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/caps/aer.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/caps/common.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/caps/common.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/caps/msi.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/caps/msi.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/caps/pcie.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/caps/pcie.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/caps/pm.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/caps/pm.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/device.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/device.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/dllp.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/dllp.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/endpoint.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/endpoint.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/function.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/function.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/msi.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/msi.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/pci.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/pci.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/port.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/port.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/rc.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/rc.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/region.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/region.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/switch.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/switch.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/tlp.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/tlp.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/core/utils.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/core/utils.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/intel/s10/__init__.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/intel/s10/__init__.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/intel/s10/interface.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/intel/s10/interface.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/intel/s10/s10_model.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/intel/s10/s10_model.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/xilinx/us/__init__.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/xilinx/us/__init__.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/xilinx/us/interface.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/xilinx/us/interface.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/xilinx/us/tlp.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/xilinx/us/tlp.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/xilinx/us/us_model.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/xilinx/us/us_model.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext/pcie/xilinx/us/usp_model.py` & `cocotbext-pcie-0.2.8/cocotbext/pcie/xilinx/us/usp_model.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/cocotbext_pcie.egg-info/PKG-INFO` & `cocotbext-pcie-0.2.8/cocotbext_pcie.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocotbext-pcie
-Version: 0.2.6
+Version: 0.2.8
 Summary: PCI express simulation framework for cocotb
 Home-page: https://github.com/alexforencich/cocotbext-pcie
 Download-URL: https://github.com/alexforencich/cocotbext-pcie/tarball/master
 Author: Alex Forencich
 Author-email: alex@alexforencich.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/alexforencich/cocotbext-pcie/issues
@@ -64,8 +64,12 @@
 
 Models of the Xilinx UltraScale and UltraScale+ PCIe hard cores are included in `cocotbext.pcie.xilinx.us`.  These modules can be used in combination with the PCIe BFM to test an HDL design that targets Xilinx UltraScale, UltraScale+, or Virtex 7 series FPGAs, up to PCIe gen 3 x16 or PCIe gen 4 x8.  The models currently only support operation as a device, not as a root port.
 
 #### Intel Stratix 10 H-Tile/L-Tile
 
 Models of the Intel Stratix 10 H-Tile/L-Tile PCIe hard cores are included in `cocotbext.pcie.intel.s10`.  These modules can be used in combination with the PCIe BFM to test an HDL design that targets Intel Stratix 10 GX, SX, TX, and MX series FPGAs that contain H-Tiles or L-Tiles, up to PCIe gen 3 x16.  The models currently only support operation as a device, not as a root port.
 
+#### Intel P-Tile
+
+Models of the Intel P-Tile PCIe hard cores are included in `cocotbext.pcie.intel.ptile`.  These modules can be used in combination with the PCIe BFM to test an HDL design that targets Intel Stratix 10 DX or Agilex F series FPGAs that contain P-Tiles, up to PCIe gen 4 x16.  The models currently only support operation as a device, not as a root port.
+
```

### Comparing `cocotbext-pcie-0.2.6/cocotbext_pcie.egg-info/SOURCES.txt` & `cocotbext-pcie-0.2.8/cocotbext_pcie.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 cocotbext/pcie/core/version.py
 cocotbext/pcie/core/caps/__init__.py
 cocotbext/pcie/core/caps/aer.py
 cocotbext/pcie/core/caps/common.py
 cocotbext/pcie/core/caps/msi.py
 cocotbext/pcie/core/caps/pcie.py
 cocotbext/pcie/core/caps/pm.py
+cocotbext/pcie/intel/ptile/__init__.py
+cocotbext/pcie/intel/ptile/interface.py
+cocotbext/pcie/intel/ptile/ptile_model.py
 cocotbext/pcie/intel/s10/__init__.py
 cocotbext/pcie/intel/s10/interface.py
 cocotbext/pcie/intel/s10/s10_model.py
 cocotbext/pcie/xilinx/us/__init__.py
 cocotbext/pcie/xilinx/us/interface.py
 cocotbext/pcie/xilinx/us/tlp.py
 cocotbext/pcie/xilinx/us/us_model.py
@@ -39,14 +42,17 @@
 cocotbext_pcie.egg-info/dependency_links.txt
 cocotbext_pcie.egg-info/requires.txt
 cocotbext_pcie.egg-info/top_level.txt
 tests/Makefile
 tests/pcie/Makefile
 tests/pcie/test_pcie.py
 tests/pcie/test_pcie.v
+tests/pcie_ptile/Makefile
+tests/pcie_ptile/test_pcie_ptile.py
+tests/pcie_ptile/test_pcie_ptile.v
 tests/pcie_s10/Makefile
 tests/pcie_s10/test_pcie_s10.py
 tests/pcie_s10/test_pcie_s10.v
 tests/pcie_us/Makefile
 tests/pcie_us/test_pcie_us.py
 tests/pcie_us/test_pcie_us.v
 tests/pcie_usp/Makefile
```

### Comparing `cocotbext-pcie-0.2.6/setup.cfg` & `cocotbext-pcie-0.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/tests/Makefile` & `cocotbext-pcie-0.2.8/tests/Makefile`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/tests/pcie/Makefile` & `cocotbext-pcie-0.2.8/tests/pcie/Makefile`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/tests/pcie/test_pcie.py` & `cocotbext-pcie-0.2.8/tests/pcie/test_pcie.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/tests/pcie_s10/Makefile` & `cocotbext-pcie-0.2.8/tests/pcie_s10/Makefile`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/tests/pcie_s10/test_pcie_s10.py` & `cocotbext-pcie-0.2.8/tests/pcie_s10/test_pcie_s10.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/tests/pcie_s10/test_pcie_s10.v` & `cocotbext-pcie-0.2.8/tests/pcie_s10/test_pcie_s10.v`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/tests/pcie_us/Makefile` & `cocotbext-pcie-0.2.8/tests/pcie_us/Makefile`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/tests/pcie_us/test_pcie_us.py` & `cocotbext-pcie-0.2.8/tests/pcie_us/test_pcie_us.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/tests/pcie_us/test_pcie_us.v` & `cocotbext-pcie-0.2.8/tests/pcie_us/test_pcie_us.v`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/tests/pcie_usp/Makefile` & `cocotbext-pcie-0.2.8/tests/pcie_usp/Makefile`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/tests/pcie_usp/test_pcie_usp.py` & `cocotbext-pcie-0.2.8/tests/pcie_usp/test_pcie_usp.py`

 * *Files identical despite different names*

### Comparing `cocotbext-pcie-0.2.6/tests/pcie_usp/test_pcie_usp.v` & `cocotbext-pcie-0.2.8/tests/pcie_usp/test_pcie_usp.v`

 * *Files identical despite different names*

