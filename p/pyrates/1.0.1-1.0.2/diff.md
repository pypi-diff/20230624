# Comparing `tmp/pyrates-1.0.1.tar.gz` & `tmp/pyrates-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrates-1.0.1.tar", last modified: Thu Apr 20 21:11:31 2023, max compression
+gzip compressed data, was "pyrates-1.0.2.tar", last modified: Sat Jun 24 19:05:39 2023, max compression
```

## Comparing `pyrates-1.0.1.tar` & `pyrates-1.0.2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.707143 pyrates-1.0.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-04-20 21:11:22.000000 pyrates-1.0.1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-04-20 21:11:22.000000 pyrates-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-20 21:11:31.703143 pyrates-1.0.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     5121 2023-04-20 21:11:22.000000 pyrates-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.695143 pyrates-1.0.1/model_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.695143 pyrates-1.0.1/model_templates/CNS_2019_Tutorial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4070 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/CNS_2019_Tutorial/templates.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/base_templates.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/model_templates/neural_mass_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/neural_mass_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/neural_mass_models/ik.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/neural_mass_models/jansenrit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/neural_mass_models/qif.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/neural_mass_models/synaptic_plasticity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/neural_mass_models/theta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/neural_mass_models/wilsoncowan.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/model_templates/oscillators/
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/oscillators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/oscillators/kuramoto.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/oscillators/stuartlandau.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/oscillators/vanderpol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/model_templates/test_resources/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/test_resources/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1581 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/test_resources/linear.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     4425 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/test_resources/test_backend.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-04-20 21:11:22.000000 pyrates-1.0.1/model_templates/test_resources/test_operator_caching_templates.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/pyrates/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/pyrates/backend/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1522 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/pyrates/backend/base/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/base/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16686 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/base/base_backend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4322 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/base/base_funcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34712 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/computegraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/pyrates/backend/fortran/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/fortran/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18865 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/fortran/fortran_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/fortran/fortran_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/pyrates/backend/julia/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/julia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/julia/julia_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/julia/julia_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/pyrates/backend/matlab/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/matlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/matlab/matlab_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/matlab/matlab_funcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26490 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/pyrates/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/tensorflow/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10410 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/tensorflow/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/tensorflow/tensorflow_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.703143 pyrates-1.0.1/pyrates/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/torch/torch_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/backend/torch/torch_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.703143 pyrates-1.0.1/pyrates/frontend/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1708 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4091 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/dict.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3302 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.703143 pyrates-1.0.1/pyrates/frontend/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/fileio/pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/fileio/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.703143 pyrates-1.0.1/pyrates/frontend/template/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5426 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/_io.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4268 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/abc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    64168 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/circuit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/circuit.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      929 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/edge.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1665 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/node.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12467 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/operator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7957 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/frontend/template/operator_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.703143 pyrates-1.0.1/pyrates/ir/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1598 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/ir/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5572 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/ir/abc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    56222 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/ir/circuit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4084 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/ir/edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7049 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/ir/node.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5162 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/ir/operator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10463 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/ir/operator_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15933 2023-04-20 21:11:22.000000 pyrates-1.0.1/pyrates/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.699143 pyrates-1.0.1/pyrates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-20 21:11:31.000000 pyrates-1.0.1/pyrates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-20 21:11:31.000000 pyrates-1.0.1/pyrates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:11:31.000000 pyrates-1.0.1/pyrates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:11:31.000000 pyrates-1.0.1/pyrates.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-20 21:11:31.000000 pyrates-1.0.1/pyrates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 21:11:31.000000 pyrates-1.0.1/pyrates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 21:11:31.707143 pyrates-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1997 2023-04-20 21:11:22.000000 pyrates-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:11:31.703143 pyrates-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-20 21:11:22.000000 pyrates-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-20 21:11:22.000000 pyrates-1.0.1/tests/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-20 21:11:22.000000 pyrates-1.0.1/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11835 2023-04-20 21:11:22.000000 pyrates-1.0.1/tests/test_backend_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22168 2023-04-20 21:11:22.000000 pyrates-1.0.1/tests/test_backend_simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-20 21:11:22.000000 pyrates-1.0.1/tests/test_file_io.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-04-20 21:11:22.000000 pyrates-1.0.1/tests/test_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-04-20 21:11:22.000000 pyrates-1.0.1/tests/test_implemented_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.037678 pyrates-1.0.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-06-24 19:05:25.000000 pyrates-1.0.2/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-06-24 19:05:25.000000 pyrates-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-24 19:05:39.037678 pyrates-1.0.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5121 2023-06-24 19:05:25.000000 pyrates-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.021678 pyrates-1.0.2/model_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.021678 pyrates-1.0.2/model_templates/CNS_2019_Tutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4070 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/CNS_2019_Tutorial/templates.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/base_templates.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.021678 pyrates-1.0.2/model_templates/neural_mass_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/neural_mass_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/neural_mass_models/ik.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/neural_mass_models/jansenrit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/neural_mass_models/qif.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/neural_mass_models/synaptic_plasticity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/neural_mass_models/theta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/neural_mass_models/wilsoncowan.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.021678 pyrates-1.0.2/model_templates/oscillators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/oscillators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/oscillators/kuramoto.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/oscillators/stuartlandau.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/oscillators/vanderpol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.025678 pyrates-1.0.2/model_templates/test_resources/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/test_resources/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1581 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/test_resources/linear.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4425 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/test_resources/test_backend.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-06-24 19:05:25.000000 pyrates-1.0.2/model_templates/test_resources/test_operator_caching_templates.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.025678 pyrates-1.0.2/pyrates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.025678 pyrates-1.0.2/pyrates/backend/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1522 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.025678 pyrates-1.0.2/pyrates/backend/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/base/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16283 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/base/base_backend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4322 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/base/base_funcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35481 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/computegraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.025678 pyrates-1.0.2/pyrates/backend/fortran/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/fortran/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18706 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/fortran/fortran_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/fortran/fortran_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.029678 pyrates-1.0.2/pyrates/backend/julia/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/julia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/julia/julia_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/julia/julia_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.029678 pyrates-1.0.2/pyrates/backend/matlab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/matlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/matlab/matlab_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/matlab/matlab_funcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26490 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.029678 pyrates-1.0.2/pyrates/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/tensorflow/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10410 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/tensorflow/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/tensorflow/tensorflow_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.029678 pyrates-1.0.2/pyrates/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/torch/torch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/backend/torch/torch_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.029678 pyrates-1.0.2/pyrates/frontend/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1708 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/frontend/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4091 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/frontend/dict.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3302 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/frontend/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.029678 pyrates-1.0.2/pyrates/frontend/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/frontend/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/frontend/fileio/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/frontend/fileio/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.033678 pyrates-1.0.2/pyrates/frontend/template/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5426 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/frontend/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/frontend/template/_io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4268 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/frontend/template/abc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    64883 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/frontend/template/circuit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/frontend/template/circuit.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/frontend/template/edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      929 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/frontend/template/edge.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1665 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/frontend/template/node.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12467 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/frontend/template/operator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7957 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/frontend/template/operator_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.033678 pyrates-1.0.2/pyrates/ir/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1598 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/ir/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5572 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/ir/abc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    56222 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/ir/circuit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4084 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/ir/edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7049 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/ir/node.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5162 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/ir/operator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10463 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/ir/operator_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15933 2023-06-24 19:05:25.000000 pyrates-1.0.2/pyrates/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.025678 pyrates-1.0.2/pyrates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-24 19:05:38.000000 pyrates-1.0.2/pyrates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-24 19:05:38.000000 pyrates-1.0.2/pyrates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 19:05:38.000000 pyrates-1.0.2/pyrates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 19:05:38.000000 pyrates-1.0.2/pyrates.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-24 19:05:38.000000 pyrates-1.0.2/pyrates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-24 19:05:38.000000 pyrates-1.0.2/pyrates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 19:05:39.037678 pyrates-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1997 2023-06-24 19:05:25.000000 pyrates-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:05:39.037678 pyrates-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-24 19:05:25.000000 pyrates-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-24 19:05:25.000000 pyrates-1.0.2/tests/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-24 19:05:25.000000 pyrates-1.0.2/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11835 2023-06-24 19:05:25.000000 pyrates-1.0.2/tests/test_backend_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22168 2023-06-24 19:05:25.000000 pyrates-1.0.2/tests/test_backend_simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-24 19:05:25.000000 pyrates-1.0.2/tests/test_file_io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-06-24 19:05:25.000000 pyrates-1.0.2/tests/test_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-06-24 19:05:25.000000 pyrates-1.0.2/tests/test_implemented_models.py
```

### Comparing `pyrates-1.0.1/LICENSE` & `pyrates-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/PKG-INFO` & `pyrates-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrates
-Version: 1.0.1
+Version: 1.0.2
 Summary: Dynamical Systems Modeling Framework
 Home-page: UNKNOWN
 Author: Richard Gast, Daniel Rose
 Author-email: richard.gast@northwestern.edu
 License: GPL v3
 Description: PyRates
         =======
```

### Comparing `pyrates-1.0.1/README.md` & `pyrates-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/model_templates/CNS_2019_Tutorial/templates.yaml` & `pyrates-1.0.2/model_templates/CNS_2019_Tutorial/templates.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/model_templates/base_templates.yaml` & `pyrates-1.0.2/model_templates/base_templates.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/model_templates/neural_mass_models/__init__.py` & `pyrates-1.0.2/model_templates/neural_mass_models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/model_templates/neural_mass_models/ik.yaml` & `pyrates-1.0.2/model_templates/neural_mass_models/ik.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/model_templates/neural_mass_models/jansenrit.yaml` & `pyrates-1.0.2/model_templates/neural_mass_models/jansenrit.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/model_templates/neural_mass_models/qif.yaml` & `pyrates-1.0.2/model_templates/neural_mass_models/qif.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/model_templates/neural_mass_models/synaptic_plasticity.yaml` & `pyrates-1.0.2/model_templates/neural_mass_models/synaptic_plasticity.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/model_templates/neural_mass_models/theta.yaml` & `pyrates-1.0.2/model_templates/neural_mass_models/theta.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/model_templates/neural_mass_models/wilsoncowan.yaml` & `pyrates-1.0.2/model_templates/neural_mass_models/wilsoncowan.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/model_templates/oscillators/__init__.py` & `pyrates-1.0.2/model_templates/oscillators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/model_templates/oscillators/kuramoto.yaml` & `pyrates-1.0.2/model_templates/oscillators/kuramoto.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/model_templates/oscillators/stuartlandau.yaml` & `pyrates-1.0.2/model_templates/oscillators/stuartlandau.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/model_templates/test_resources/linear.yaml` & `pyrates-1.0.2/model_templates/test_resources/linear.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/model_templates/test_resources/test_backend.yaml` & `pyrates-1.0.2/model_templates/test_resources/test_backend.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/model_templates/test_resources/test_operator_caching_templates.yml` & `pyrates-1.0.2/model_templates/test_resources/test_operator_caching_templates.yml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/__init__.py` & `pyrates-1.0.2/pyrates/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,12 +28,12 @@
 # Richard Gast and Daniel Rose et. al. in preparation
 """Python package for building and simulating complex dynamical systems. Represents the dynamical systems as graphs,
 i.e. networks of nodes connected via edges.
 """
 
 __author__ = "Richard Gast, Daniel Rose"
 __status__ = "Development"
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 
 from pyrates.utility import integrate, grid_search, clear_frontend_caches, clear
 from pyrates.frontend import CircuitTemplate, NodeTemplate, EdgeTemplate, OperatorTemplate, save
```

### Comparing `pyrates-1.0.1/pyrates/backend/__init__.py` & `pyrates-1.0.2/pyrates/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/base/__init__.py` & `pyrates-1.0.2/pyrates/backend/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/base/base_backend.py` & `pyrates-1.0.2/pyrates/backend/base/base_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -328,36 +328,26 @@
         decorator = kwargs.pop('decorator', None)
         if decorator:
             decorator_kwargs = kwargs.pop('decorator_kwargs', dict())
             rhs_eval = decorator(rhs_eval, **decorator_kwargs)
 
         return rhs_eval
 
-    def run(self, func: Callable, func_args: tuple, T: float, dt: float, dts: float, outputs: dict,
-            solver: str, **kwargs) -> dict:
+    def run(self, func: Callable, func_args: tuple, T: float, dt: float, dts: float, solver: str, **kwargs) -> tuple:
 
         # initial values
         t0 = func_args[0]
         times = np.arange(0.0, T, dts) if dts else np.arange(0.0, T, dt)
         y0 = func_args[1]
 
         # perform simulation
         results = self._solve(solver=solver, func=func, args=func_args[2:], T=T, dt=dt, dts=dts, y0=y0, t0=t0,
                               times=times, **kwargs)
 
-        # reduce state recordings to requested state variables
-        for key, idx in outputs.items():
-            if type(idx) is tuple and idx[1] - idx[0] == 1:
-                idx = (idx[0],)
-            elif type(idx) is int:
-                idx = (idx,)
-            outputs[key] = results[:, idx] if len(idx) == 1 else results[:, idx[0]:idx[1]]
-        outputs['time'] = times
-
-        return outputs
+        return results, times
 
     def clear(self):
 
         # clear code generator
         super().clear()
 
         # remove files and directories that have been created during simulation process
```

### Comparing `pyrates-1.0.1/pyrates/backend/base/base_funcs.py` & `pyrates-1.0.2/pyrates/backend/base/base_funcs.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/computegraph.py` & `pyrates-1.0.2/pyrates/backend/computegraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -450,31 +450,43 @@
                 fargs.append(arg)
             else:
                 fargs.append(self.get_var(arg, from_backend=True))
 
         return func, tuple(fargs), tuple(func_args), self._state_var_indices.copy()
 
     def run(self, func: Callable, func_args: tuple, T: float, dt: float, dts: Optional[float] = None,
-            outputs: Optional[dict] = None, **kwargs):
+            outputs: Optional[dict] = None, **kwargs) -> dict:
 
         # pre-process outputs
         if outputs is None:
             outputs = {key: key for key in self.state_vars}
         for key in outputs.copy():
             var = outputs.pop(key)
             outputs[key] = self._state_var_indices[var]
 
         # handle other arguments
         if dts is None:
             dts = dt
         solver = kwargs.pop('solver', 'euler')
 
         # call backend method
-        return self.backend.run(func=func, func_args=func_args, T=T, dt=dt, dts=dts, outputs=outputs, solver=solver,
-                                **kwargs)
+        results, times = self.backend.run(func=func, func_args=func_args, T=T, dt=dt, dts=dts, solver=solver, **kwargs)
+
+        # set state variables to final simulated value
+        for key in self.state_vars:
+            var = self.get_var(key)
+            idx = self._state_var_indices[key]
+            var.set_value(np.reshape(self._index_state_var(results, idx)[-1], var.shape))
+
+        # reduce state recordings to requested state variables
+        for key, idx in outputs.items():
+            outputs[key] = self._index_state_var(results, idx)
+        outputs['time'] = times
+
+        return outputs
 
     def clear(self) -> None:
         """Deletes build directory and removes all compute graph nodes
         """
 
         # delete network nodes and variables from the compute graph
         for n in list(self.nodes.keys()):
@@ -883,14 +895,22 @@
             except ValueError:
                 new_label = f"{label}_0"
             return self._generate_unique_label(new_label)
         else:
             return label
 
     @staticmethod
+    def _index_state_var(y: np.ndarray, idx: Union[int, tuple, list]) -> np.ndarray:
+        if type(idx) is tuple and idx[1] - idx[0] == 1:
+            idx = (idx[0],)
+        elif type(idx) is int:
+            idx = (idx,)
+        return y[:, idx] if len(idx) == 1 else y[:, idx[0]:idx[1]]
+
+    @staticmethod
     def _process_func_call(expr: str, func: str, replacement: str):
 
         # identify start and end of the function call
         start = expr.find(f"{func}(")
         end = expr[start:].find(')') + 1
 
         # replace part in expression string
```

### Comparing `pyrates-1.0.1/pyrates/backend/fortran/__init__.py` & `pyrates-1.0.2/pyrates/backend/fortran/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/fortran/fortran_backend.py` & `pyrates-1.0.2/pyrates/backend/fortran/fortran_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,22 +287,23 @@
         self.add_code_line("integer, intent(in) :: ndim, icp(*), ijac")
         self.add_code_line(f"{dtype}, intent(in) :: y(ndim), args(*)")
         self.add_code_line(f"{dtype}, intent(out) :: dy(ndim)")
         self.add_code_line(f"{dtype}, intent(inout) :: dfdu(ndim,ndim), dfdp(ndim,*)")
 
         # extract parameters from args list
         increment = 1
-        params = []
+        params, param_indices = [], []
         for i, arg in enumerate(func_args):
             idx = i + increment
             if blocked_indices[0] <= idx <= blocked_indices[1]:
                 idx -= increment
                 increment += blocked_indices[1] - blocked_indices[0]
                 idx += increment
             params.append(f'args({idx})')
+            param_indices.append(idx)
 
         # call the pyrates subroutine
         additional_args = f", {', '.join(params)}" if params else ""
         self.add_linebreak()
         self.add_code_line(f"call {func_name}(args(14), y, dy{additional_args})")
         self.add_linebreak()
         self.add_code_line("end subroutine func")
@@ -319,20 +320,15 @@
         self.add_code_line("integer, intent(in) :: ndim")
         self.add_code_line(f"{dtype}, intent(inout) :: y(ndim), args(*)")
         self.add_code_line(f"{dtype}, intent(in) :: t")
         self.add_linebreak()
 
         # define parameter values
         increment = 1
-        for i, arg in enumerate(func_args):
-            idx = i + increment
-            if blocked_indices[0] <= idx <= blocked_indices[1]:
-                idx -= increment
-                increment += blocked_indices[1] - blocked_indices[0]
-                idx += increment
+        for idx, arg in zip(param_indices, func_args):
             p = self._var_declaration_info[arg]
             if sum(p.shape) > 1:
                 raise ValueError(f'Vector-valued parameter detected ({p.name} with shape {p.shape}), which cannot be '
                                  f'handled by Auto-07p. Please change the definition of your network (e.g. remove '
                                  f'extrinsic inputs) such that no vectorized model parameters exist.')
             self.add_code_line(f"args({idx}) = {p.value}  ! {p.name}")
 
@@ -365,15 +361,15 @@
         auto_constants = {'NDIM': 1, 'NPAR': 1, 'IPS': -2, 'ILP': 0, 'ICP': [14], 'NTST': 1, 'NCOL': 3, 'IAD': 0,
                           'ISP': 0, 'ISW': 1, 'IPLT': 0, 'NBC': 0, 'NINT': 0, 'NMX': 10000, 'NPR': 1, 'MXBF': 10,
                           'IID': 2, 'ITMX': 2, 'ITNW': 5, 'NWTN': 2, 'JAC': 0, 'EPSL': 1e-6, 'EPSU': 1e-6, 'EPSS': 1e-4,
                           'IRS': 0, 'DS': 1e-4, 'DSMIN': 1e-8, 'DSMAX': 1e-2, 'IADS': 1, 'THL': {}, 'THU': {},
                           'UZR': {}, 'STOP': {}}
 
         auto_constants['NDIM'] = len(state_vars)
-        auto_constants['NPAR'] = len(func_args)
+        auto_constants['NPAR'] = max(param_indices)
         for key in list(kwargs.keys()):
             if key in auto_constants:
                 auto_constants[key] = kwargs.pop(key)
 
         # write auto constants to string
         for key, val in auto_constants.items():
             self.add_code_line(f"{key} = {val}")
```

### Comparing `pyrates-1.0.1/pyrates/backend/fortran/fortran_funcs.py` & `pyrates-1.0.2/pyrates/backend/fortran/fortran_funcs.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/julia/__init__.py` & `pyrates-1.0.2/pyrates/backend/julia/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/julia/julia_backend.py` & `pyrates-1.0.2/pyrates/backend/julia/julia_backend.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/julia/julia_funcs.py` & `pyrates-1.0.2/pyrates/backend/julia/julia_funcs.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/matlab/__init__.py` & `pyrates-1.0.2/pyrates/backend/matlab/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/matlab/matlab_backend.py` & `pyrates-1.0.2/pyrates/backend/matlab/matlab_backend.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/matlab/matlab_funcs.py` & `pyrates-1.0.2/pyrates/backend/matlab/matlab_funcs.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/parser.py` & `pyrates-1.0.2/pyrates/backend/parser.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/tensorflow/__init__.py` & `pyrates-1.0.2/pyrates/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/tensorflow/tensorflow_backend.py` & `pyrates-1.0.2/pyrates/backend/tensorflow/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/tensorflow/tensorflow_funcs.py` & `pyrates-1.0.2/pyrates/backend/tensorflow/tensorflow_funcs.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/torch/__init__.py` & `pyrates-1.0.2/pyrates/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/torch/torch_backend.py` & `pyrates-1.0.2/pyrates/backend/torch/torch_backend.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/backend/torch/torch_funcs.py` & `pyrates-1.0.2/pyrates/backend/torch/torch_funcs.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/frontend/__init__.py` & `pyrates-1.0.2/pyrates/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/frontend/dict.py` & `pyrates-1.0.2/pyrates/frontend/dict.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/frontend/file.py` & `pyrates-1.0.2/pyrates/frontend/file.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/frontend/fileio/__init__.py` & `pyrates-1.0.2/pyrates/frontend/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/frontend/fileio/yaml.py` & `pyrates-1.0.2/pyrates/frontend/fileio/yaml.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/frontend/template/__init__.py` & `pyrates-1.0.2/pyrates/frontend/template/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/frontend/template/_io.py` & `pyrates-1.0.2/pyrates/frontend/template/_io.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/frontend/template/abc.py` & `pyrates-1.0.2/pyrates/frontend/template/abc.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/frontend/template/circuit.py` & `pyrates-1.0.2/pyrates/frontend/template/circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,24 +134,29 @@
 
         # private attributes
         self._ir = None
         self._depth = self._get_hierarchy_depth()
         self._vectorization_labels = {}
         self._vectorization_indices = {}
         self._state_var_indices = {}
+        self._state_var_values = {}
 
     def __getitem__(self, item):
         """Attempts to return the node with name `item`.
         """
         try:
             return self.nodes[item]
         except KeyError:
             warn(PyRatesWarning(f"Node with name {item} was not found on {self.name}."))
             return
 
+    @property
+    def state(self):
+        return self._state_var_values
+
     def to_yaml(self, path, **kwargs) -> None:
         """Shorthand to save the `CircuitTemplate` to a yaml file. After that call, either a new YAML file has been
         created including all template definitions required to reconstruct the `CircuitTemplate` instance, or additional
         operators have been added to the already existing YAML file.
 
         Parameters
         ----------
@@ -503,14 +508,19 @@
             else:
                 columns.append(key)
                 data.append(out)
         if multi_index:
             columns = MultiIndex.from_tuples(columns)
         results = DataFrame(data=np.asarray(data).T, columns=columns, index=time_vec)
 
+        # store current state of the network
+        for key in net.compute_graph.state_vars:
+            self._state_var_values[key] = net.compute_graph.get_var(key).value
+
+        # clean up
         if clear:
             net.clear()
         self._ir = net._ir
 
         return results.loc[cutoff:, :]
 
     def get_run_func(self, func_name: str, step_size: float, inputs: Optional[dict] = None, backend: str = None,
@@ -572,19 +582,29 @@
         # validate backend settings
         net._validate_backend_args(backend, vectorize, **kwargs)
 
         # translate circuit template into a graph representation
         net.apply(adaptive_steps=adaptive_steps, verbose=verbose, backend=backend, step_size=step_size,
                   vectorize=vectorize, **kwargs)
 
+        # impose initial condition
+        for key, val in self._state_var_values.items():
+            v = net.compute_graph.get_var(key)
+            v.set_value(np.reshape(val, v.shape))
+
         # generate the run function
         func, args, arg_names, state_var_indices = net._ir.get_run_func(func_name=func_name, step_size=step_size,
                                                                         **kwargs)
         self._state_var_indices = state_var_indices
 
+        # set current network state if it was empty before
+        if not self.state:
+            for key in net.compute_graph.state_vars:
+                self._state_var_values[key] = net.compute_graph.get_var(key).value
+
         # clear the network temporary files
         if clear:
             net.clear()
         self._ir = net._ir
 
         # map the backend variable names to the frontend variable names
         state_var_map = {}
```

### Comparing `pyrates-1.0.1/pyrates/frontend/template/edge.py` & `pyrates-1.0.2/pyrates/frontend/template/edge.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/frontend/template/edge.yaml` & `pyrates-1.0.2/pyrates/frontend/template/edge.yaml`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/frontend/template/node.py` & `pyrates-1.0.2/pyrates/frontend/template/node.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/frontend/template/operator.py` & `pyrates-1.0.2/pyrates/frontend/template/operator.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/frontend/template/operator_graph.py` & `pyrates-1.0.2/pyrates/frontend/template/operator_graph.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/ir/__init__.py` & `pyrates-1.0.2/pyrates/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/ir/abc.py` & `pyrates-1.0.2/pyrates/ir/abc.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/ir/circuit.py` & `pyrates-1.0.2/pyrates/ir/circuit.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/ir/edge.py` & `pyrates-1.0.2/pyrates/ir/edge.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/ir/node.py` & `pyrates-1.0.2/pyrates/ir/node.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/ir/operator.py` & `pyrates-1.0.2/pyrates/ir/operator.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/ir/operator_graph.py` & `pyrates-1.0.2/pyrates/ir/operator_graph.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates/utility.py` & `pyrates-1.0.2/pyrates/utility.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/pyrates.egg-info/PKG-INFO` & `pyrates-1.0.2/pyrates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrates
-Version: 1.0.1
+Version: 1.0.2
 Summary: Dynamical Systems Modeling Framework
 Home-page: UNKNOWN
 Author: Richard Gast, Daniel Rose
 Author-email: richard.gast@northwestern.edu
 License: GPL v3
 Description: PyRates
         =======
```

### Comparing `pyrates-1.0.1/pyrates.egg-info/SOURCES.txt` & `pyrates-1.0.2/pyrates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/setup.py` & `pyrates-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/tests/__init__.py` & `pyrates-1.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/tests/benchmarks.py` & `pyrates-1.0.2/tests/benchmarks.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/tests/conftest.py` & `pyrates-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/tests/test_backend_parser.py` & `pyrates-1.0.2/tests/test_backend_parser.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/tests/test_backend_simulations.py` & `pyrates-1.0.2/tests/test_backend_simulations.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/tests/test_file_io.py` & `pyrates-1.0.2/tests/test_file_io.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/tests/test_frontend.py` & `pyrates-1.0.2/tests/test_frontend.py`

 * *Files identical despite different names*

### Comparing `pyrates-1.0.1/tests/test_implemented_models.py` & `pyrates-1.0.2/tests/test_implemented_models.py`

 * *Files identical despite different names*

