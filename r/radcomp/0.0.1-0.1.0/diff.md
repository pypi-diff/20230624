# Comparing `tmp/radcomp-0.0.1.tar.gz` & `tmp/radcomp-0.1.0.tar.gz`

## Comparing `radcomp-0.0.1.tar` & `radcomp-0.1.0.tar`

### file list

```diff
@@ -1,68 +1,75 @@
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 radcomp-0.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 radcomp-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 radcomp-0.0.1/CITATION.cff
--rw-r--r--   0        0        0    52355 2020-02-02 00:00:00.000000 radcomp-0.0.1/poetry.lock
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 radcomp-0.0.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 radcomp-0.0.1/docs/make.bat
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 radcomp-0.0.1/docs/requirements.txt
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 radcomp-0.0.1/docs/source/conf.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 radcomp-0.0.1/docs/source/index.rst
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 radcomp-0.0.1/docs/source/modules.rst
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 radcomp-0.0.1/docs/source/overview.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 radcomp-0.0.1/docs/source/radcomp.common.prelayer.rst
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 radcomp-0.0.1/docs/source/radcomp.common.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 radcomp-0.0.1/docs/source/radcomp.common.utils.rst
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 radcomp-0.0.1/docs/source/radcomp.dcm.dcm.rst
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 radcomp-0.0.1/docs/source/radcomp.dcm.dcm_internal.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 radcomp-0.0.1/docs/source/radcomp.dcm.dcm_read_toml.rst
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 radcomp-0.0.1/docs/source/radcomp.dcm.rst
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 radcomp-0.0.1/docs/source/radcomp.rst
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 radcomp-0.0.1/examples/example.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 radcomp-0.0.1/examples/example.toml
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 radcomp-0.0.1/examples/example_with_prelayer.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 radcomp-0.0.1/examples/example_with_prelayer.toml
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 radcomp-0.0.1/src/radcomp/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 radcomp-0.0.1/src/radcomp/common/__init__.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 radcomp-0.0.1/src/radcomp/common/prelayer.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 radcomp-0.0.1/src/radcomp/common/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 radcomp-0.0.1/src/radcomp/dcm/__init__.py
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 radcomp-0.0.1/src/radcomp/dcm/dcm.py
--rw-r--r--   0        0        0    19984 2020-02-02 00:00:00.000000 radcomp-0.0.1/src/radcomp/dcm/dcm_internal.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 radcomp-0.0.1/src/radcomp/dcm/dcm_read_toml.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/common/test_prelayer.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/common/test_utils.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/sympy-ode-solver.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/test_dcm.py
--rw-r--r--   0        0        0    43105 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/test_dcm_cases.py
--rw-r--r--   0        0        0    10597 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/test_dcm_internal.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/test_dcm_read_toml.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg1-itac.toml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg1.toml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg10-itac.toml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg10.toml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg11-itac.toml
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg11.toml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg2-itac.toml
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg2.toml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg3-itac.toml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg3.toml
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg4-itac.toml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg4.toml
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg5.toml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg6.toml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg7.toml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg8.toml
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-eg9.toml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-exp-ac225.toml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-exp-parallel-layers.toml
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-linearity-1cmpt.toml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-linearity-itac.toml
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-linearity-ncmpt.toml
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-read.toml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-stable-parallel.toml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 radcomp-0.0.1/test/dcm/tomls-for-testing/test-stable.toml
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 radcomp-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 radcomp-0.0.1/LICENSE
--rw-r--r--   0        0        0     7753 2020-02-02 00:00:00.000000 radcomp-0.0.1/README.md
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 radcomp-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     8600 2020-02-02 00:00:00.000000 radcomp-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 radcomp-0.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 radcomp-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 radcomp-0.1.0/CITATION.cff
+-rw-r--r--   0        0        0    52355 2020-02-02 00:00:00.000000 radcomp-0.1.0/poetry.lock
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 radcomp-0.1.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 radcomp-0.1.0/docs/make.bat
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 radcomp-0.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 radcomp-0.1.0/docs/source/conf.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 radcomp-0.1.0/docs/source/index.rst
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 radcomp-0.1.0/docs/source/modules.rst
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 radcomp-0.1.0/docs/source/overview.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 radcomp-0.1.0/docs/source/radcomp.common.prelayer.rst
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 radcomp-0.1.0/docs/source/radcomp.common.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 radcomp-0.1.0/docs/source/radcomp.common.utils.rst
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 radcomp-0.1.0/docs/source/radcomp.common.voiding.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 radcomp-0.1.0/docs/source/radcomp.dcm.dcm.rst
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 radcomp-0.1.0/docs/source/radcomp.dcm.dcm_internal.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 radcomp-0.1.0/docs/source/radcomp.dcm.dcm_read_toml.rst
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 radcomp-0.1.0/docs/source/radcomp.dcm.rst
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 radcomp-0.1.0/docs/source/radcomp.rst
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 radcomp-0.1.0/examples/example.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 radcomp-0.1.0/examples/example.toml
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 radcomp-0.1.0/examples/example_prelayer.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 radcomp-0.1.0/examples/example_prelayer.toml
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 radcomp-0.1.0/examples/example_voiding.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 radcomp-0.1.0/examples/example_voiding.toml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 radcomp-0.1.0/src/radcomp/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 radcomp-0.1.0/src/radcomp/common/__init__.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 radcomp-0.1.0/src/radcomp/common/prelayer.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 radcomp-0.1.0/src/radcomp/common/utils.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 radcomp-0.1.0/src/radcomp/common/voiding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 radcomp-0.1.0/src/radcomp/dcm/__init__.py
+-rw-r--r--   0        0        0    12871 2020-02-02 00:00:00.000000 radcomp-0.1.0/src/radcomp/dcm/dcm.py
+-rw-r--r--   0        0        0    27974 2020-02-02 00:00:00.000000 radcomp-0.1.0/src/radcomp/dcm/dcm_internal.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 radcomp-0.1.0/src/radcomp/dcm/dcm_read_toml.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/common/test_prelayer.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/common/test_utils.py
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/common/test_voiding.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/sympy-ode-solver.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/test_dcm.py
+-rw-r--r--   0        0        0    51743 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/test_dcm_cases.py
+-rw-r--r--   0        0        0    18032 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/test_dcm_internal.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/test_dcm_read_toml.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg1-itac.toml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg1.toml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg10-itac.toml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg10.toml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg11-itac.toml
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg11.toml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg2-itac.toml
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg2.toml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg3-itac.toml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg3.toml
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg4-itac.toml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg4.toml
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg5.toml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg6.toml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg7.toml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg8.toml
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-eg9.toml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-exp-ac225.toml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-exp-parallel-layers.toml
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-linearity-1cmpt.toml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-linearity-itac.toml
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-linearity-ncmpt.toml
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-read.toml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-stable-parallel.toml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-stable.toml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-voiding-2l1c.toml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 radcomp-0.1.0/test/dcm/tomls-for-testing/test-voiding-2l2c.toml
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 radcomp-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 radcomp-0.1.0/LICENSE
+-rw-r--r--   0        0        0     8731 2020-02-02 00:00:00.000000 radcomp-0.1.0/README.md
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 radcomp-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9578 2020-02-02 00:00:00.000000 radcomp-0.1.0/PKG-INFO
```

### Comparing `radcomp-0.0.1/.readthedocs.yaml` & `radcomp-0.1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/poetry.lock` & `radcomp-0.1.0/poetry.lock`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/docs/Makefile` & `radcomp-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/docs/make.bat` & `radcomp-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/docs/source/conf.py` & `radcomp-0.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/examples/example.toml` & `radcomp-0.1.0/examples/example.toml`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/examples/example_with_prelayer.py` & `radcomp-0.1.0/examples/example_prelayer.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,13 +22,11 @@
         lambda t: radcomp.nuclei_to_activity(n2(t), trans_rate),
         lambda t: radcomp.nuclei_to_activity(n3(t), trans_rate),
     ],
     "Radionuclide 1",
 )
 
 t_eval = np.linspace(0, 24, 1000)  # h
-model = radcomp.solve_dcm_from_toml(
-    "example_with_prelayer.toml", t_eval, prelayer=prelayer
-)
+model = radcomp.solve_dcm_from_toml("example_prelayer.toml", t_eval, prelayer=prelayer)
 print(model.info_xfer())
 print(model.info_growth())
 model.plot()
```

### Comparing `radcomp-0.0.1/src/radcomp/common/prelayer.py` & `radcomp-0.1.0/src/radcomp/common/prelayer.py`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/src/radcomp/common/utils.py` & `radcomp-0.1.0/src/radcomp/common/utils.py`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/src/radcomp/dcm/dcm.py` & `radcomp-0.1.0/src/radcomp/dcm/dcm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
 import numpy as np
 from typing import Optional
 
 from radcomp.common.utils import nuclei_to_activity, _save_arrays
 from radcomp.common.prelayer import Prelayer
+from radcomp.common.voiding import VoidingRule
 from radcomp.dcm.dcm_internal import (
     _include_prelayer_in_branching_frac,
     _solve_dcm,
     _plot_solved_tacs,
     _cumulated_activity,
     _info_xfer,
     _info_growth,
@@ -47,26 +48,32 @@
         Number of layers in model (excluding any prelayer).
     num_compartments: int
         Number of compartments in model.
     nuclei : numpy.ndarray
         Shape (``num_layers``, ``num_compartments``, len(``t_eval``)). The solution.
         Element [i, j, k] is the number of nuclei in layer i, compartment j
         at element k of ``t_eval``.
+    voided_nuclei : list[numpy.ndarray]
+        Element i is a 3D array containing the number of nuclei voided
+        due to the ith voiding rule. This 3D array has shape
+        (number of voiding times in ith voiding rule, ``num_layers``, ``num_compartments``).
+        See also :func:`voided_activity`.
     """
 
     trans_rates: np.ndarray
     branching_fracs: np.ndarray
     xfer_coeffs: np.ndarray
     t_eval: np.ndarray
     prelayer: Prelayer | None
     layer_names: list[str] | None
     compartment_names: list[str] | None
     num_layers: int
     num_compartments: int
     nuclei: np.ndarray
+    voided_nuclei: list[np.ndarray]
 
     def activity(self) -> np.ndarray:
         """Activities (MBq) at times in ``t_eval``.
 
         Returns
         -------
         numpy.ndarray
@@ -77,25 +84,67 @@
         return np.array(
             [
                 nuclei_to_activity(yl, tr)
                 for yl, tr in zip(self.nuclei, self.trans_rates)
             ]
         )
 
-    def cumulated_activity(self) -> np.ndarray:
+    def voided_activity(self):
+        """Activities (MBq) voided due to voiding rules.
+
+        See also ``voided_nuclei``.
+
+        Returns
+        -------
+        list[numpy.ndarray]
+            Element i is a 3D array containing the activity (MBq) voided
+            due to the ith voiding rule. This 3D array has shape
+            (number of voiding times in voiding rule i, ``num_layers``, ``num_compartments``).
+        """
+        return [
+            np.transpose(
+                np.array(
+                    [
+                        nuclei_to_activity(x, tr)
+                        for x, tr in zip(np.transpose(vnr, (1, 0, 2)), self.trans_rates)
+                    ]
+                ),
+                (1, 0, 2),
+            )
+            for vnr in self.voided_nuclei
+        ]
+
+    def cumulated_activity(
+        self,
+        t_start: Optional[float] = None,
+        t_end: Optional[float] = None,
+    ) -> np.ndarray:
         """Cumulated activity (MBq h) during ``t_eval``.
 
+        Note result is sensitive to choice of ``t_eval``.
+
+        Parameters
+        ----------
+        t_start : Optional[float]
+            Start time (h) of integration. Default is start of ``t_eval``.
+        t_end : Optional[float]
+            End time (h) of integration. Default is end of ``t_eval``.
+
         Returns
         -------
         numpy.ndarray
             Shape (``num_layers``, ``num_compartments``). Element at index [i, j] is the
-            cumulated activity (MBq h) in layer i, compartment j during ``t_eval``.
+            cumulated activity (MBq h) in layer i, compartment j from ``t_start`` to ``t_end``.
         """
         return _cumulated_activity(
-            [self.t_eval] * self.num_layers, self.nuclei, self.trans_rates
+            [self.t_eval] * self.num_layers,
+            self.nuclei,
+            self.trans_rates,
+            t_start=t_start,
+            t_end=t_end,
         )
 
     def halflife(self) -> np.ndarray:
         """Half-lives (h) of nuclides in layers.
 
         Stable nuclides are assigned a half-life of numpy.inf.
 
@@ -209,14 +258,15 @@
     branching_fracs: np.ndarray,
     xfer_coeffs: np.ndarray,
     initial_nuclei: np.ndarray,
     t_eval: np.ndarray,
     prelayer: Optional[Prelayer] = None,
     layer_names: Optional[list[str]] = None,
     compartment_names: Optional[list[str]] = None,
+    voiding_rules: Optional[list[VoidingRule]] = None,
 ) -> DetCompModelSol:
     """Solve a deterministic compartment model.
 
     For more information about the model, see
     https://github.com/jakeforster/radcomp/blob/main/README.md.
 
     Parameters
@@ -227,20 +277,23 @@
         Branching fractions (0 to 1). Shape (``num_layers``, ``num_layers``). Element [i, j] is for layer j to layer i.
     xfer_coeffs : numpy.ndarray
         Transfer coefficients (h-1) between compartments. Shape (``num_layers``, ``num_compartments``, ``num_compartments``). Element [i, j, k] is for compartment k to compartment j in layer i.
     initial_nuclei : numpy.ndarray
         Number of nuclei in each compartment in each layer at first element of ``t_eval``. Shape (``num_layers``, ``num_compartments``). Element [i, j] is for layer i, compartment j.
     t_eval : numpy.ndarray
         Times (h) at which to solve the model. Must be sorted (ascending).
+        Note the first element is the beginning of the integration period.
     prelayer : Optional[Prelayer]
         Input time-activity curves for a nuclide that is able to transition to one or more layers in the model.
     layer_names : Optional[list[str]]
         Names of layers in model.
     compartment_names : Optional[list[str]]
         Names of compartments in model.
+    voiding_rules : Optional[list[VoidingRule]]
+        Rules for voiding nuclei from compartments.
 
     Returns
     -------
     DetCompModelSol
         Solution for the model.
     """
 
@@ -249,59 +302,66 @@
         branching_fracs,
         xfer_coeffs,
         initial_nuclei,
         t_eval,
         prelayer,
         layer_names,
         compartment_names,
+        voiding_rules,
     )
     num_layers, num_compartments, _ = xfer_coeffs.shape
     t_span = (t_eval.min(), t_eval.max())
-    _, nuclei = _solve_dcm(
+    _, nuclei, voided_nuclei = _solve_dcm(
         t_span,
         initial_nuclei,
         trans_rates,
         branching_fracs,
         xfer_coeffs,
         t_eval=t_eval,
         prelayer_as_tuple=_prelayer_as_tuple(prelayer, num_layers, num_compartments),
+        voiding_rules=voiding_rules,
     )
     return DetCompModelSol(
         trans_rates,
         branching_fracs,
         xfer_coeffs,
         t_eval,
         prelayer,
         layer_names,
         compartment_names,
         num_layers,
         num_compartments,
         np.array(nuclei),
+        voided_nuclei,
     )
 
 
 def solve_dcm_from_toml(
     filepath: str,
     t_eval: np.ndarray,
     prelayer: Optional[Prelayer] = None,
+    voiding_rules: Optional[list[VoidingRule]] = None,
 ) -> DetCompModelSol:
     """Solve a deterministic compartment model from a
     TOML configuration file (except for a possible prelayer).
 
     For more information about the model or how to format the
     TOML file, see https://github.com/jakeforster/radcomp/blob/main/README.md.
 
     Parameters
     ----------
     filepath : str
         Filepath to TOML configuration file.
     t_eval : np.ndarray
         Times (h) at which to solve the model. Must be sorted (ascending).
+        Note the first element is the beginning of the integration period.
     prelayer : Optional[Prelayer]
         Input time-activity curves for a nuclide that is able to transition to one or more layers in the model.
+    voiding_rules : Optional[list[VoidingRule]]
+        Rules for voiding nuclei from compartments.
 
     Returns
     -------
     DetCompModelSol
         Solution for the model.
     """
     (
@@ -317,8 +377,9 @@
         branching_fracs,
         xfer_coeffs,
         initial_nuclei,
         t_eval,
         prelayer=prelayer,
         layer_names=layer_names,
         compartment_names=compartment_names,
+        voiding_rules=voiding_rules,
     )
```

### Comparing `radcomp-0.0.1/src/radcomp/dcm/dcm_internal.py` & `radcomp-0.1.0/src/radcomp/dcm/dcm_internal.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 import matplotlib.pyplot as plt
 from scipy.interpolate import interp1d
 from collections.abc import Callable
 from typing import Optional
 
 from radcomp.common.utils import nuclei_to_activity
 from radcomp.common.prelayer import Prelayer
+from radcomp.common.voiding import (
+    VoidingRule,
+    _VoidingEvent,
+    _create_time_ordered_voids_for_layer,
+)
 
 
 def _prelayer_as_tuple(
     prelayer: Prelayer | None,
     num_layers: int,
     num_compartments: int,
 ) -> tuple[float, np.ndarray, list[Callable[[float], float]]]:
@@ -50,14 +55,15 @@
     branching_fracs: np.ndarray,
     xfer_coeffs: np.ndarray,
     initial_nuclei: np.ndarray,
     t_eval: np.ndarray,
     prelayer: Optional[Prelayer] = None,
     layer_names: Optional[list[str]] = None,
     compartment_names: Optional[list[str]] = None,
+    voiding_rules: Optional[list[VoidingRule]] = None,
 ) -> None:
     """Assert statements to check validity of input parameters
     for deterministic compartment model.
 
     Parameters
     ----------
     trans_rates : numpy.ndarray
@@ -72,14 +78,15 @@
         Times (h) at which to solve the model. Must be sorted (ascending).
     prelayer : Optional[radcomp.Prelayer]
         Input time-activity curves for a nuclide that is able to transition to one or more layers in the model.
     layer_names : Optional[list[str]]
         Names of layers in model.
     compartment_names : Optional[list[str]]
         Names of compartments in model.
+    voiding_rules: Optiona[list[VoidingRule]]
     """
 
     # size checks
     a, b, c = xfer_coeffs.shape
     assert b == c
     num_layers = a
     num_compartments = b
@@ -89,14 +96,19 @@
     if prelayer is not None:
         assert prelayer.branching_fracs.shape == (num_layers,)
         assert len(prelayer.activity_funcs) == num_compartments
     if layer_names is not None:
         assert len(layer_names) == num_layers
     if compartment_names is not None:
         assert len(compartment_names) == num_compartments
+    if voiding_rules is not None:
+        assert all(
+            rule.fractions.shape == (num_layers, num_compartments)
+            for rule in voiding_rules
+        )
 
     # some type checks
     if prelayer is not None:
         assert all(callable(yp) for yp in prelayer.activity_funcs)
 
     # content checks
     assert np.all(xfer_coeffs >= 0)
@@ -125,26 +137,172 @@
                     )
                 )
                 >= 0
             )
             for act in prelayer.activity_funcs
         )
 
+    if voiding_rules is not None:
+        assert all(
+            all(t_span[0] <= time <= t_span[1] for time in rule.times)
+            for rule in voiding_rules
+        )
+
+
+def _solve_dcm_layer(
+    layer: int,
+    t_span: tuple[float, float] | list[float],
+    initial_nuclei_layer: np.ndarray,
+    trans_rates_new: np.ndarray,
+    branching_fracs_new: np.ndarray,
+    xfer_coeffs_new: np.ndarray,
+    nuclei_funcs: list[list[Callable[[float], float]]],
+    time_ordered_voids_for_layer: list[_VoidingEvent],
+    t_eval: Optional[np.ndarray] = None,
+) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
+    """Solve a layer of the deterministic compartment model.
+
+    Note the layers of the model may include a prelayer.
+    So num_layers may be 1 more than expected.
+
+    Parameters
+    ----------
+    layer : int
+        Layer of model being solved. Never the prelayer.
+    t_span : tuple[float, float] | list[float]
+        2-member sequence. Interval of integration (h).
+    initial_nuclei_layer : numpy.ndarray
+        Number of nuclei in each compartment of the layer at `t_eval[0]`. Shape (num_compartments,).
+    trans_rates_new : numpy.ndarray
+        Transition rates (h-1) of nuclides in layers. Shape (num_layers,).
+    branching_fracs_new : numpy.ndarray
+        Branching fractions (0 to 1). Shape (num_layers, num_layers). `branching_fracs_new`[i,j] is for layer j to layer i.
+    xfer_coeffs_new : numpy.ndarray
+        Transfer coefficients (h-1) between compartments. Shape (num_layers, num_compartments, num_compartments). `xfer_coeffs_new`[i,j,k] is for compartment k to compartment j in layer i.
+    nuclei_funcs : list[list[Callable[[float], float]]]
+        Length `layer`. `nuclei_funcs`[i] is the number of layer i nuclei
+        as a function of time (h) for each compartment in model;
+        length num_compartments; element at index j is the function for compartment j.
+    time_ordered_voids_for_layer : list[_VoidingEvent]
+    t_eval : Optional[numpy.ndarray]
+        Times (h) at which to solve the model. Must be sorted (ascending). Must be within `t_span`.
+
+    Returns
+    -------
+    tuple[list[np.ndarray], list[np.ndarray], list[np.ndarray]]
+        + 1D array of times (h) at which layer is solved.
+          If `t_eval` is provided, this is `t_eval`.
+        + 2D array containing the solution for layer.
+          This 2D array has shape (num_compartments, len(first_out[i])),
+          where first_out is the first element of the return tuple.
+        + Shape (len(`time_ordered_voids_for_layer`), num_compartments).
+          Element [i,j] is the number of nuclei voided in compartment j
+          in ith element of `time_ordered_voids_for_layer`.
+    """
+
+    _, b, c = xfer_coeffs_new.shape
+    assert b == c
+    num_compartments = b
+
+    t_start = t_span[0]
+
+    sol_t_layer = np.empty(0)
+    sol_y_layer = np.empty((num_compartments, 0))
+    num_voids = len(time_ordered_voids_for_layer)
+    voided_nuclei_layer = np.zeros((num_voids, num_compartments))
+    for i, voiding_event in enumerate(time_ordered_voids_for_layer):
+        t_end = voiding_event.time
+        assert t_end <= t_span[1]
+
+        # slice t_eval
+        t_eval_interval = (
+            None
+            if t_eval is None
+            else np.append(t_eval[(t_eval >= t_start) & (t_eval < t_end)], [t_end])
+        )
+        # if t_eval is None, t_span bounds are always included in the deduced t_eval in solve_ivp
+
+        # solve
+        sol = solve_ivp(
+            _ode_rhs,
+            (t_start, t_end),
+            initial_nuclei_layer,
+            t_eval=t_eval_interval,
+            args=(
+                trans_rates_new,
+                branching_fracs_new[layer],
+                xfer_coeffs_new[layer],
+                layer,
+                nuclei_funcs,
+            ),
+        )
+
+        # record number of nuclei voided at t_end
+        voided_nuclei = sol.y[:, -1] * voiding_event.fractions
+        voided_nuclei_layer[i] = voided_nuclei
+
+        # initial conditions for next interval
+        initial_nuclei_layer = sol.y[:, -1] - voided_nuclei
+
+        # store soln with end point modified to account for void
+        sol_t_layer = np.append(sol_t_layer, sol.t)
+        sol_y_layer = np.append(sol_y_layer, sol.y[:, :-1], axis=1)
+        sol_y_layer = np.concatenate(
+            (sol_y_layer, np.reshape(initial_nuclei_layer, (-1, 1))), axis=1
+        )
+
+        # get ready for next interval
+        t_start = t_end
+
+    # final interval
+    if t_start != t_span[1]:
+        t_eval_interval = None if t_eval is None else t_eval[t_eval >= t_start]
+        sol = solve_ivp(
+            _ode_rhs,
+            (t_start, t_span[1]),
+            initial_nuclei_layer,
+            t_eval=t_eval_interval,
+            args=(
+                trans_rates_new,
+                branching_fracs_new[layer],
+                xfer_coeffs_new[layer],
+                layer,
+                nuclei_funcs,
+            ),
+        )
+
+        # store soln extending to t_span[1]
+        sol_t_layer = np.append(sol_t_layer, sol.t)
+        sol_y_layer = np.append(sol_y_layer, sol.y, axis=1)
+
+    # drop duplicates at void times
+    sol_t_layer, indices = np.unique(sol_t_layer, return_index=True)
+    sol_y_layer = sol_y_layer[:, indices]
+
+    # drop time points at void times if they are not in t_eval
+    if t_eval is not None:
+        mask = np.isin(sol_t_layer, t_eval)
+        sol_t_layer = sol_t_layer[mask]
+        sol_y_layer = sol_y_layer[:, mask]
+
+    return sol_t_layer, sol_y_layer, voided_nuclei_layer
+
 
 def _solve_dcm(
     t_span: tuple[float, float] | list[float],
     initial_nuclei: np.ndarray,
     trans_rates: np.ndarray,
     branching_fracs: np.ndarray,
     xfer_coeffs: np.ndarray,
     t_eval: Optional[np.ndarray] = None,
     prelayer_as_tuple: Optional[
         tuple[float, np.ndarray, list[Callable[[float], float]]]
     ] = None,
-) -> tuple[list[np.ndarray], list[np.ndarray]]:
+    voiding_rules: Optional[list[VoidingRule]] = None,
+) -> tuple[list[np.ndarray], list[np.ndarray], list[np.ndarray]]:
     """Solve the deterministic compartment model.
 
     Parameters
     ----------
     t_span : tuple[float, float] | list[float]
         2-member sequence. Interval of integration (h).
     initial_nuclei : numpy.ndarray
@@ -159,25 +317,30 @@
         Times (h) at which to solve the model. Must be sorted (ascending). Must be within `t_span`.
     prelayer_as_tuple : Optional[ tuple[float, np.ndarray, list[Callable[[float], float]]] ]
         + Transition rate (h-1) for nuclide in prelayer.
         + Branching fractions (0 to 1). Shape (`num_layers`,).
           `branching_fracs`[i] is for prelayer to layer i in model.
         + Number of prelayer nuclei as a function of time (h) for
           each compartment in the model. Length `num_compartments`.
+    voiding_rules : Optional[list[VoidingRule]]
 
     Returns
     -------
-    tuple[list[np.ndarray], list[np.ndarray]]
+    tuple[list[np.ndarray], list[np.ndarray], list[np.ndarray]]
         + Length num_layers. Element i is the 1D array of
           times (h) at which layer i is solved. If `t_eval`
-          is not provided, this is [`t_eval`] * num_layers.
+          is provided, this is [`t_eval`] * num_layers.
         + Length num_layers. Element i is a 2D array containing
           the solution for layer i. This 2D array has
           shape (num_compartments, len(first_out[i])), where
           first_out is the first element of the return tuple.
+        + Length len(`voiding_rules`). Element i is a 3D array
+          containing the number of nuclei voided due to
+          ith element of `voiding_rules`. This 3D array has shape
+          (len(voiding_rules[i].times), num_layers, num_compartments).
     """
 
     t_layers = []
     nuclei_layers = []
     nuclei_funcs = []
 
     num_layers, b, c = xfer_coeffs.shape
@@ -192,48 +355,70 @@
         (
             trans_rate_prelayer,
             branching_frac_prelayer,
             nuclei_funcs_prelayer,
         ) = prelayer_as_tuple
     nuclei_funcs.append(nuclei_funcs_prelayer)
 
+    if voiding_rules is None:
+        voiding_rules = []
+
     (
         initial_nuclei_new,
         trans_rates_new,
         branching_fracs_new,
         xfer_coeffs_new,
+        voiding_rules_new,
     ) = _include_prelayer(
         initial_nuclei,
         trans_rates,
         branching_fracs,
         xfer_coeffs,
         trans_rate_prelayer,
         branching_frac_prelayer,
+        voiding_rules,
     )
 
     num_layers_new = len(trans_rates_new)
+
+    voided_nuclei_new = [
+        np.zeros((len(rule.times), num_layers_new, num_compartments))
+        for rule in voiding_rules_new
+    ]
+
     for layer in range(1, num_layers_new):
-        sol = solve_ivp(
-            _ode_rhs,
+        time_ordered_voids_for_layer = _create_time_ordered_voids_for_layer(
+            voiding_rules_new, layer
+        )
+        sol_t_layer, sol_y_layer, voided_nuclei_layer = _solve_dcm_layer(
+            layer,
             t_span,
             initial_nuclei_new[layer],
+            trans_rates_new,
+            branching_fracs_new,
+            xfer_coeffs_new,
+            nuclei_funcs,
+            time_ordered_voids_for_layer,
             t_eval=t_eval,
-            args=(
-                trans_rates_new,
-                branching_fracs_new[layer],
-                xfer_coeffs_new[layer],
-                layer,
-                nuclei_funcs,
-            ),
         )
-        t_layers.append(sol.t)
-        nuclei_layers.append(sol.y)
-        nuclei_funcs.append([interp1d(sol.t, n) for n in sol.y])
 
-    return t_layers, nuclei_layers
+        for voiding_event, voided_nuclei_layer_event in zip(
+            time_ordered_voids_for_layer, voided_nuclei_layer
+        ):
+            voided_nuclei_new[voiding_event.voiding_rules_index][
+                voiding_event.voiding_rule_times_index,
+                layer,
+            ] = voided_nuclei_layer_event
+
+        t_layers.append(sol_t_layer)
+        nuclei_layers.append(sol_y_layer)
+        nuclei_funcs.append([interp1d(sol_t_layer, n) for n in sol_y_layer])
+
+    voided_nuclei = [x[:, 1:, :] for x in voided_nuclei_new]
+    return t_layers, nuclei_layers, voided_nuclei
 
 
 def _ode_rhs(
     t: float,
     nuclei: np.ndarray,
     trans_rates: np.ndarray,
     branching_fracs_layer: np.ndarray,
@@ -288,15 +473,16 @@
 def _include_prelayer(
     initial_nuclei: np.ndarray,
     trans_rates: np.ndarray,
     branching_fracs: np.ndarray,
     xfer_coeffs: np.ndarray,
     trans_rate_prelayer: float,
     branching_fracs_prelayer: np.ndarray,
-) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
+    voiding_rules: list[VoidingRule],
+) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, list[VoidingRule]]:
     """Make parameters for deterministic compartment model
     include the prelayer.
 
     Parameters
     ----------
     initial_nuclei : numpy.ndarray
         Number of nuclei in each compartment in each layer at `t_eval`[0]. Shape (num_layers, num_compartments). `initial_nuclei`[i,j] is for layer i, compartment j.
@@ -325,15 +511,31 @@
         trans_rates.astype(float, casting="safe"), 0, trans_rate_prelayer
     )
     branching_fracs_new = _include_prelayer_in_branching_frac(
         branching_fracs, branching_fracs_prelayer
     )
     initial_nuclei_new = np.insert(initial_nuclei, 0, 0, axis=0)
     xfer_coeffs_new = np.insert(xfer_coeffs, 0, 0, axis=0)
-    return initial_nuclei_new, trans_rates_new, branching_fracs_new, xfer_coeffs_new
+    voiding_rules_new = _include_prelayer_in_voiding_rules(voiding_rules)
+    return (
+        initial_nuclei_new,
+        trans_rates_new,
+        branching_fracs_new,
+        xfer_coeffs_new,
+        voiding_rules_new,
+    )
+
+
+def _include_prelayer_in_voiding_rules(
+    voiding_rules: list[VoidingRule],
+) -> list[VoidingRule]:
+    return [
+        VoidingRule(rule.times, np.insert(rule.fractions, 0, 0, axis=0))
+        for rule in voiding_rules
+    ]
 
 
 def _include_prelayer_in_branching_frac(
     branching_fracs: np.ndarray, branching_fracs_prelayer: np.ndarray
 ) -> np.ndarray:
     """Make branching_fracs parameter for deterministic compartment
     model include the prelayer.
@@ -362,15 +564,15 @@
 
 def _plot_solved_tacs(
     t_layers: list[np.ndarray],
     nuclei_layers: list[np.ndarray] | np.ndarray,
     trans_rates: np.ndarray,
     layer_names: Optional[list[str]] = None,
     compartment_names: Optional[list[str]] = None,
-):
+) -> None:
     """Produce plots of time-activity curves or time-nuclei curves.
 
     Parameters
     ----------
     t_layers : list[numpy.ndarray]
         Length num_layers. `t_layers`[i] is the 1D array of
         times (h) at which layer i is solved.
@@ -415,14 +617,16 @@
     plt.show()
 
 
 def _cumulated_activity(
     t_layers: list[np.ndarray],
     nuclei_layers: list[np.ndarray] | np.ndarray,
     trans_rates: np.ndarray,
+    t_start: Optional[float] = None,
+    t_end: Optional[float] = None,
 ) -> np.ndarray:
     """Cumulated activity (MBq h).
 
     Parameters
     ----------
     t_layers : list[numpy.ndarray]
         Length num_layers. `t_layers`[i] is the 1D array of
@@ -442,16 +646,33 @@
     """
 
     num_layers = len(trans_rates)
     assert num_layers == len(t_layers)
     num_compartments = len(nuclei_layers[0])
     ans = np.zeros((num_layers, num_compartments))
     for layer, (tc, nl) in enumerate(zip(t_layers, nuclei_layers)):
+
+        if t_start is not None:
+            assert t_start >= tc[0]
+            t_start_l = t_start
+        else:
+            t_start_l = tc[0]
+
+        if t_end is not None:
+            assert t_end <= tc[-1]
+            t_end_l = t_end
+        else:
+            t_end_l = tc[-1]
+
+        mask = (tc >= t_start_l) & (tc <= t_end_l)
+
         for i, nc in enumerate(nl):
-            ans[layer, i] = np.trapz(nuclei_to_activity(nc, trans_rates[layer]), x=tc)
+            ans[layer, i] = np.trapz(
+                nuclei_to_activity(nc[mask], trans_rates[layer]), x=tc[mask]
+            )
     return ans
 
 
 def _info_xfer(
     xfer_coeffs: np.ndarray,
     layer_names: Optional[list[str]] = None,
     compartment_names: Optional[list[str]] = None,
```

### Comparing `radcomp-0.0.1/src/radcomp/dcm/dcm_read_toml.py` & `radcomp-0.1.0/src/radcomp/dcm/dcm_read_toml.py`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/test/common/test_prelayer.py` & `radcomp-0.1.0/test/common/test_prelayer.py`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/test/common/test_utils.py` & `radcomp-0.1.0/test/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/test/dcm/sympy-ode-solver.py` & `radcomp-0.1.0/test/dcm/sympy-ode-solver.py`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/test/dcm/test_dcm.py` & `radcomp-0.1.0/test/dcm/test_dcm.py`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/test/dcm/test_dcm_cases.py` & `radcomp-0.1.0/test/dcm/test_dcm_cases.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import os
 
 from radcomp.common.utils import nuclei_to_activity
 from radcomp.common.prelayer import Prelayer
 from radcomp.dcm.dcm import solve_dcm, solve_dcm_from_toml
 from radcomp.dcm.dcm_read_toml import _dcm_read_toml
+from radcomp.common.voiding import VoidingRule
 
 toml_dir = os.path.join(os.path.dirname(__file__), "tomls-for-testing")
 
 
 def test_const():
     """
     1 stable nuclide, 1 compartment
@@ -1492,7 +1493,278 @@
         fp,
         t_eval + 2313.4,
     )
     assert np.allclose(
         model.activity()[0][0],
         model_shift.activity()[0][0],
     )
+
+
+def test_voiding_2l1c():
+    """99Mo to 99mTc generator.
+
+    + initially 10 GBq of 99Mo
+    + 99mTc is eluted at 0 h, 24 h, 48 h
+
+    99Mo to 99mTc branching fraction is 0.89
+
+    activity of 99mTc reaches its maximum value:
+    a = branching_frac * activity 99Mo
+    at this time after elution:
+    t = (trans rate 99Mo - trans rate 99mTc)^(-1)
+    * ln(trans rate 99Mo / trans rate 99mTc )
+    """
+    trans_rates = np.array([0.010502, 0.115525])
+    voiding_rule = VoidingRule(np.array([24, 48]), np.array([[0], [1]]))
+    voiding_rules = [voiding_rule]
+    t_max = (trans_rates[0] - trans_rates[1]) ** (-1) * np.log(
+        trans_rates[0] / trans_rates[1]
+    )
+    assert t_max < voiding_rule.times[0]
+    assert t_max < voiding_rule.times[1] - voiding_rule.times[0]
+    t_eval = np.sort(
+        np.append(
+            np.append(np.linspace(0, 72, 1000), voiding_rule.times + t_max), t_max
+        )
+    )
+    fp = os.path.join(toml_dir, "test-voiding-2l1c.toml")
+    model = solve_dcm_from_toml(fp, t_eval, voiding_rules=voiding_rules)
+
+    mask = t_eval == t_max
+    assert np.isclose(
+        model.activity()[1, 0, mask], model.activity()[0, 0, mask] * 0.89, rtol=0.00009
+    )
+
+    mask = t_eval == voiding_rules[0].times[0]
+    assert np.isclose(model.activity()[1, 0, mask], 0, rtol=0.0001)
+
+    mask = t_eval == voiding_rules[0].times[0] + t_max
+    assert np.isclose(
+        model.activity()[1, 0, mask], model.activity()[0, 0, mask] * 0.89, rtol=0.00008
+    )
+
+    mask = t_eval == voiding_rules[0].times[1]
+    assert np.isclose(model.activity()[1, 0, mask], 0, rtol=0.0001)
+
+    mask = t_eval == voiding_rules[0].times[1] + t_max
+    assert np.isclose(
+        model.activity()[1, 0, mask], model.activity()[0, 0, mask] * 0.89, rtol=0.00009
+    )
+
+    # void at 24 h
+    activity_voided_24h = (
+        0.89
+        * trans_rates[1]
+        / (trans_rates[1] - trans_rates[0])
+        * model.activity()[0, 0, t_eval == voiding_rules[0].times[0]]
+        * (1 - np.exp(-(trans_rates[1] - trans_rates[0]) * voiding_rules[0].times[0]))
+    )[0]
+
+    # void at 48 h
+    activity_voided_48h = (
+        0.89
+        * trans_rates[1]
+        / (trans_rates[1] - trans_rates[0])
+        * model.activity()[0, 0, t_eval == voiding_rules[0].times[1]]
+        * (
+            1
+            - np.exp(
+                -(trans_rates[1] - trans_rates[0])
+                * (voiding_rules[0].times[1] - voiding_rules[0].times[0])
+            )
+        )
+    )[0]
+
+    voided_activity = model.voided_activity()
+    assert len(voided_activity) == 1
+    assert voided_activity[0].shape == (2, 2, 1)
+    assert np.allclose(
+        voided_activity[0],
+        np.array([[[0], [activity_voided_24h]], [[0], [activity_voided_48h]]]),
+        rtol=8e-5,
+    )
+
+
+def test_voiding_2l1c_v2():
+    """99Mo to 99mTc generator.
+
+    + initially 10 GBq of 99Mo
+    + 99mTc is eluted at 0 h, 24 h, 48 h
+
+    99Mo to 99mTc branching fraction is 0.89
+
+    activity of 99mTc reaches its maximum value:
+    a = branching_frac * activity 99Mo
+    at this time after elution:
+    t = (trans rate 99Mo - trans rate 99mTc)^(-1)
+    * ln(trans rate 99Mo / trans rate 99mTc )
+    """
+    trans_rates = np.array([0.010502, 0.115525])
+    voiding_rules = [
+        VoidingRule(np.array([48]), np.array([[0], [1]])),
+        VoidingRule(np.array([24]), np.array([[0], [1]])),
+    ]
+    t_max = (trans_rates[0] - trans_rates[1]) ** (-1) * np.log(
+        trans_rates[0] / trans_rates[1]
+    )
+    assert t_max < voiding_rules[1].times[0]
+    assert t_max < voiding_rules[0].times[0] - voiding_rules[1].times[0]
+    t_eval = np.sort(
+        np.append(
+            np.append(np.linspace(0, 72, 1000), np.array([24, 48]) + t_max), t_max
+        )
+    )
+    fp = os.path.join(toml_dir, "test-voiding-2l1c.toml")
+    model = solve_dcm_from_toml(fp, t_eval, voiding_rules=voiding_rules)
+
+    mask = t_eval == t_max
+    assert np.isclose(
+        model.activity()[1, 0, mask], model.activity()[0, 0, mask] * 0.89, rtol=0.00009
+    )
+
+    mask = t_eval == 24
+    assert np.isclose(model.activity()[1, 0, mask], 0, rtol=0.0001)
+
+    mask = t_eval == 24 + t_max
+    assert np.isclose(
+        model.activity()[1, 0, mask], model.activity()[0, 0, mask] * 0.89, rtol=0.00008
+    )
+
+    mask = t_eval == 48
+    assert np.isclose(model.activity()[1, 0, mask], 0, rtol=0.0001)
+
+    mask = t_eval == 48 + t_max
+    assert np.isclose(
+        model.activity()[1, 0, mask], model.activity()[0, 0, mask] * 0.89, rtol=0.00009
+    )
+
+    # void at 24 h
+    activity_voided_24h = (
+        0.89
+        * trans_rates[1]
+        / (trans_rates[1] - trans_rates[0])
+        * model.activity()[0, 0, t_eval == 24]
+        * (1 - np.exp(-(trans_rates[1] - trans_rates[0]) * 24))
+    )[0]
+
+    # void at 48 h
+    activity_voided_48h = (
+        0.89
+        * trans_rates[1]
+        / (trans_rates[1] - trans_rates[0])
+        * model.activity()[0, 0, t_eval == 48]
+        * (1 - np.exp(-(trans_rates[1] - trans_rates[0]) * 24))
+    )[0]
+
+    voided_activity = model.voided_activity()
+    assert len(voided_activity) == 2
+    assert voided_activity[0].shape == (1, 2, 1)
+    assert np.allclose(
+        voided_activity[0],
+        np.array([[[0], [activity_voided_48h]]]),
+        rtol=7e-5,
+    )
+
+    # assert activity_voided_24h == 0  # 6996.974
+    # assert activity_voided_48h == 0  # 5438.02
+    voided_activity = model.voided_activity()
+    assert voided_activity[1].shape == (1, 2, 1)
+    assert np.allclose(
+        voided_activity[1],
+        np.array([[[0], [activity_voided_24h]]]),
+        rtol=8e-5,
+    )
+
+
+def test_voiding_2l2c():
+    """99Mo to 99mTc generator, but there is 1 compartment
+    representing the generator and another compartment
+    that is independent of the first.
+
+    compartment 1:
+    + initially 10 GBq of 99Mo
+    + 99mTc is eluted at 0 h, 24 h, 48 h
+
+    compartment 2:
+    + initially 10 GBq of 99Mo
+
+    No xfer between compartments in either layer
+
+    99Mo to 99mTc branching fraction is 0.89
+
+    activity of 99mTc reaches its maximum value:
+    a = branching_frac * activity 99Mo
+    at this time after elution:
+    t = (trans rate 99Mo - trans rate 99mTc)^(-1)
+    * ln(trans rate 99Mo / trans rate 99mTc )
+    """
+    trans_rates = np.array([0.010502, 0.115525])
+    voiding_rule = VoidingRule(np.array([24, 48]), np.array([[0, 0], [1, 0]]))
+    voiding_rules = [voiding_rule]
+    t_max = (trans_rates[0] - trans_rates[1]) ** (-1) * np.log(
+        trans_rates[0] / trans_rates[1]
+    )
+    t_eval = np.sort(
+        np.append(
+            np.append(np.linspace(0, 72, 1000), voiding_rule.times + t_max), t_max
+        )
+    )
+    fp = os.path.join(toml_dir, "test-voiding-2l2c.toml")
+    model = solve_dcm_from_toml(fp, t_eval, voiding_rules=voiding_rules)
+
+    # compartment 1
+    mask = t_eval == t_max
+    assert np.isclose(
+        model.activity()[1, 0, mask], model.activity()[0, 0, mask] * 0.89, rtol=0.00009
+    )
+
+    mask = t_eval == voiding_rules[0].times[0] + t_max
+    assert np.isclose(
+        model.activity()[1, 0, mask], model.activity()[0, 0, mask] * 0.89, rtol=0.0001
+    )
+
+    mask = t_eval == voiding_rules[0].times[1] + t_max
+    assert np.isclose(
+        model.activity()[1, 0, mask], model.activity()[0, 0, mask] * 0.89, rtol=0.00017
+    )
+
+    # compartment 2
+    A1 = lambda t: 1e4 * np.exp(-trans_rates[0] * t)
+    A2 = (
+        lambda t: A1(t)
+        * 0.89
+        * (trans_rates[1] / (trans_rates[1] - trans_rates[0]))
+        * (1 - np.exp(-(trans_rates[1] - trans_rates[0]) * t))
+    )
+    assert np.allclose(model.activity()[0, 1], A1(t_eval), rtol=2e-5)
+    assert np.allclose(model.activity()[1, 1], A2(t_eval), rtol=2e-4)
+
+    # void at 24 h
+    activity_voided_24h = (
+        0.89
+        * trans_rates[1]
+        / (trans_rates[1] - trans_rates[0])
+        * model.activity()[0, 0, t_eval == 24]
+        * (1 - np.exp(-(trans_rates[1] - trans_rates[0]) * 24))
+    )[0]
+
+    # void at 48 h
+    activity_voided_48h = (
+        0.89
+        * trans_rates[1]
+        / (trans_rates[1] - trans_rates[0])
+        * model.activity()[0, 0, t_eval == 48]
+        * (1 - np.exp(-(trans_rates[1] - trans_rates[0]) * 24))
+    )[0]
+
+    voided_activity = model.voided_activity()
+    # assert activity_voided_24h == 0  # 6996.974
+    # assert activity_voided_48h == 0  # 5438.02
+    assert len(voided_activity) == 1
+    assert voided_activity[0].shape == (2, 2, 2)
+    assert np.allclose(
+        voided_activity[0],
+        np.array(
+            [[[0, 0], [activity_voided_24h, 0]], [[0, 0], [activity_voided_48h, 0]]]
+        ),
+        rtol=9e-5,
+    )
```

### Comparing `radcomp-0.0.1/test/dcm/test_dcm_read_toml.py` & `radcomp-0.1.0/test/dcm/test_dcm_read_toml.py`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/test/dcm/tomls-for-testing/test-linearity-1cmpt.toml` & `radcomp-0.1.0/test/dcm/tomls-for-testing/test-linearity-1cmpt.toml`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/test/dcm/tomls-for-testing/test-linearity-itac.toml` & `radcomp-0.1.0/test/dcm/tomls-for-testing/test-linearity-itac.toml`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/test/dcm/tomls-for-testing/test-linearity-ncmpt.toml` & `radcomp-0.1.0/test/dcm/tomls-for-testing/test-linearity-ncmpt.toml`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/test/dcm/tomls-for-testing/test-read.toml` & `radcomp-0.1.0/test/dcm/tomls-for-testing/test-read.toml`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/.gitignore` & `radcomp-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/LICENSE` & `radcomp-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radcomp-0.0.1/README.md` & `radcomp-0.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![DOI](https://zenodo.org/badge/634282475.svg)](https://zenodo.org/badge/latestdoi/634282475)
+
 # Radcomp: Radioactive compartment models
 
 Radcomp is a Python package for modelling the movement of radioactive nuclei and their progeny through a system. 
 
 Currently only deterministic compartment models are provided. 
 
 ## Requires
@@ -73,14 +75,16 @@
 | `name`            | Name of layer                                              |                |                                                      | String                                        | No                                                           |
 
 Table 1: Layer keys for a DCM. Here $a$ is the index of the layer (1-based index), $m$ is the number of layers, and $n$ is the number of compartments.
 
 Note:
 + The values in `xfer_coeffs_h-1`, `initial_MBq`, and `initial_nuclei` are in order of compartments.
 + The first value in `branching_fracs` is for the transition to the layer immediately below. 
++ The initial values `initial_nuclei` and `initial_MBq` are the values at the start of the integration period.
+
 To check the input was as intended, call the `info_xfer()` and `info_growth()` methods of the `DetCompModelSol` instance.
 
 An example of a TOML file for a DCM is provided below. 
 
 ``` toml
 [compartments]
 names = ["Organ 1", "Organ 2", "Organ 3"]
@@ -116,24 +120,36 @@
 
 The user has the option to supply time-activity curves (TACs) for a nuclide that is able to transition to one or more layers in the model. 
 The TACs in the "prelayer" can then contribute to the growth of nuclei in layers. 
 If a prelayer is provided, prelayer TACs must be provided for all compartments. 
 
 Unlike the layers in the model, the prelayer is **not** specified in the input TOML file. 
 Instead, pass an instance of the `Prelayer` class to the instantiating model method (e.g. `solve_dcm_from_toml()`) using the optional keyword argument `prelayer`.
+See [examples](https://github.com/jakeforster/radcomp/tree/main/examples) and refer to the [API reference](https://radcomp.readthedocs.io).
+
+## Voiding
+*(New in Version 0.1.0)*
+
+The user has the option to void nuclei from compartments at times during the integration period.
+This is specified by "voiding rules".
+
+Create one or more instances of the `VoidingRule` class and pass them to the instantiating model method (e.g. `solve_dcm_from_toml()`) using the optional keyword argument `voiding_rules`.
+The number of nuclei and activity voided are also recorded in the `DetCompModelSol` instance.
+See [examples](https://github.com/jakeforster/radcomp/tree/main/examples) and refer to the [API reference](https://radcomp.readthedocs.io).
 
 ## API reference
 
 https://radcomp.readthedocs.io
 
-## Examples 
+## Examples
 
 https://github.com/jakeforster/radcomp/tree/main/examples
 
 ## Testing
 
     python -m pytest
 
 ## TODO
 
-Add stochastic models
+- Add support for forcing functions
+- Stochastic models
```

### Comparing `radcomp-0.0.1/pyproject.toml` & `radcomp-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # LSP
 [tool.pyright]
-venv = "venv3.11.2"
+venv = "venv3.11"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "radcomp"
-version = "0.0.1"
+version = "0.1.0"
 authors = [{ name = "Jake Forster" },]
 description = "Model the movement of radioactive nuclei and their progeny through a system"
 readme = "README.md"
 requires-python = ">=3.10, <3.12"
 license = { text = "MIT" }
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -30,15 +30,15 @@
 Homepage = "https://github.com/jakeforster/radcomp"
 "Bug Tracker" = "https://github.com/jakeforster/radcomp/issues"
 Documentation = "https://radcomp.readthedocs.io"
 Changelog = "https://github.com/jakeforster/radcomp/CHANGELOG.md"
 
 [tool.poetry]
 name = "radcomp"
-version = "0.0.1"
+version = "0.1.0"
 description = "Model the movement of radioactive nuclei and their progeny through a system"
 authors = ["Jake Forster <jakecameron.forster@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jakeforster/radcomp"
 repository = "https://github.com/jakeforster/radcomp"
 documentation = "https://radcomp.readthedocs.io"
```

### Comparing `radcomp-0.0.1/PKG-INFO` & `radcomp-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radcomp
-Version: 0.0.1
+Version: 0.1.0
 Summary: Model the movement of radioactive nuclei and their progeny through a system
 Project-URL: Homepage, https://github.com/jakeforster/radcomp
 Project-URL: Bug Tracker, https://github.com/jakeforster/radcomp/issues
 Project-URL: Documentation, https://radcomp.readthedocs.io
 Project-URL: Changelog, https://github.com/jakeforster/radcomp/CHANGELOG.md
 Author: Jake Forster
 License: MIT
@@ -15,14 +15,16 @@
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: <3.12,>=3.10
 Requires-Dist: matplotlib<4,>=3.7.1
 Requires-Dist: numpy<2,>=1.24.2
 Requires-Dist: scipy<2,>=1.10.1
 Description-Content-Type: text/markdown
 
+[![DOI](https://zenodo.org/badge/634282475.svg)](https://zenodo.org/badge/latestdoi/634282475)
+
 # Radcomp: Radioactive compartment models
 
 Radcomp is a Python package for modelling the movement of radioactive nuclei and their progeny through a system. 
 
 Currently only deterministic compartment models are provided. 
 
 ## Requires
@@ -94,14 +96,16 @@
 | `name`            | Name of layer                                              |                |                                                      | String                                        | No                                                           |
 
 Table 1: Layer keys for a DCM. Here $a$ is the index of the layer (1-based index), $m$ is the number of layers, and $n$ is the number of compartments.
 
 Note:
 + The values in `xfer_coeffs_h-1`, `initial_MBq`, and `initial_nuclei` are in order of compartments.
 + The first value in `branching_fracs` is for the transition to the layer immediately below. 
++ The initial values `initial_nuclei` and `initial_MBq` are the values at the start of the integration period.
+
 To check the input was as intended, call the `info_xfer()` and `info_growth()` methods of the `DetCompModelSol` instance.
 
 An example of a TOML file for a DCM is provided below. 
 
 ``` toml
 [compartments]
 names = ["Organ 1", "Organ 2", "Organ 3"]
@@ -137,24 +141,36 @@
 
 The user has the option to supply time-activity curves (TACs) for a nuclide that is able to transition to one or more layers in the model. 
 The TACs in the "prelayer" can then contribute to the growth of nuclei in layers. 
 If a prelayer is provided, prelayer TACs must be provided for all compartments. 
 
 Unlike the layers in the model, the prelayer is **not** specified in the input TOML file. 
 Instead, pass an instance of the `Prelayer` class to the instantiating model method (e.g. `solve_dcm_from_toml()`) using the optional keyword argument `prelayer`.
+See [examples](https://github.com/jakeforster/radcomp/tree/main/examples) and refer to the [API reference](https://radcomp.readthedocs.io).
+
+## Voiding
+*(New in Version 0.1.0)*
+
+The user has the option to void nuclei from compartments at times during the integration period.
+This is specified by "voiding rules".
+
+Create one or more instances of the `VoidingRule` class and pass them to the instantiating model method (e.g. `solve_dcm_from_toml()`) using the optional keyword argument `voiding_rules`.
+The number of nuclei and activity voided are also recorded in the `DetCompModelSol` instance.
+See [examples](https://github.com/jakeforster/radcomp/tree/main/examples) and refer to the [API reference](https://radcomp.readthedocs.io).
 
 ## API reference
 
 https://radcomp.readthedocs.io
 
-## Examples 
+## Examples
 
 https://github.com/jakeforster/radcomp/tree/main/examples
 
 ## Testing
 
     python -m pytest
 
 ## TODO
 
-Add stochastic models
+- Add support for forcing functions
+- Stochastic models
```

