# Comparing `tmp/chgnet-0.1.3.tar.gz` & `tmp/chgnet-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chgnet-0.1.3.tar", last modified: Sat May  6 09:35:08 2023, max compression
+gzip compressed data, was "chgnet-0.1.4.tar", last modified: Sat Jun 24 04:56:41 2023, max compression
```

## Comparing `chgnet-0.1.3.tar` & `chgnet-0.1.4.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.189251 chgnet-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-06 09:34:58.000000 chgnet-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-05-06 09:35:08.189251 chgnet-0.1.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     9380 2023-05-06 09:34:58.000000 chgnet-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.181251 chgnet-0.1.3/chgnet/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.181251 chgnet-0.1.3/chgnet/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29046 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.181251 chgnet-0.1.3/chgnet/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/graph/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/graph/crystalgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    13346 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/graph/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.181251 chgnet-0.1.3/chgnet/model/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/model/basis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12947 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/model/composition_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/model/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/model/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/model/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16021 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/model/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    32417 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.181251 chgnet-0.1.3/chgnet/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)  4639235 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/pretrained/e30f77s348m32.pth.tar
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.185251 chgnet-0.1.3/chgnet/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26910 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/trainer/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.181251 chgnet-0.1.3/chgnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-05-06 09:35:08.000000 chgnet-0.1.3/chgnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-06 09:35:08.000000 chgnet-0.1.3/chgnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 09:35:08.000000 chgnet-0.1.3/chgnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-06 09:35:08.000000 chgnet-0.1.3/chgnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-06 09:35:08.000000 chgnet-0.1.3/chgnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-06 09:34:58.000000 chgnet-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 09:35:08.189251 chgnet-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.189251 chgnet-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_crystal_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_relaxation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.570674 chgnet-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-24 04:56:31.000000 chgnet-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-06-24 04:56:41.570674 chgnet-0.1.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9357 2023-06-24 04:56:31.000000 chgnet-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.558674 chgnet-0.1.4/chgnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.558674 chgnet-0.1.4/chgnet/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30798 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.558674 chgnet-0.1.4/chgnet/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/graph/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/graph/crystalgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14447 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/graph/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.562674 chgnet-0.1.4/chgnet/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/model/basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/model/composition_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20235 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/model/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/model/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/model/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16042 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32348 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.562674 chgnet-0.1.4/chgnet/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)  4639235 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/pretrained/e30f77s348m32.pth.tar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.566674 chgnet-0.1.4/chgnet/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27116 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.570674 chgnet-0.1.4/chgnet/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/utils/vasp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.558674 chgnet-0.1.4/chgnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-06-24 04:56:41.000000 chgnet-0.1.4/chgnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-24 04:56:41.000000 chgnet-0.1.4/chgnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 04:56:41.000000 chgnet-0.1.4/chgnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-24 04:56:41.000000 chgnet-0.1.4/chgnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 04:56:41.000000 chgnet-0.1.4/chgnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-24 04:56:31.000000 chgnet-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 04:56:41.570674 chgnet-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.570674 chgnet-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_crystal_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_trainer.py
```

### Comparing `chgnet-0.1.3/LICENSE` & `chgnet-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.3/PKG-INFO` & `chgnet-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: chgnet
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pretrained Universal Neural Network Potential for Charge-informed Atomistic Modeling
 Author-email: Bowen Deng <bowendeng@berkeley.edu>
 License: Modified BSD
 Project-URL: Source, https://github.com/CederGroupHub/chgnet
 Project-URL: Package, https://pypi.org/project/chgnet
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Chemistry
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: crystal-toolkit
 License-File: LICENSE
 
@@ -28,14 +28,15 @@
 
 [![Tests](https://github.com/CederGroupHub/chgnet/actions/workflows/test.yml/badge.svg)](https://github.com/CederGroupHub/chgnet/actions/workflows/test.yml)
 [![Linting](https://github.com/CederGroupHub/chgnet/actions/workflows/lint.yml/badge.svg)](https://github.com/CederGroupHub/chgnet/actions/workflows/lint.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/e3bdcea0382a495d96408e4f84408e85)](https://app.codacy.com/gh/CederGroupHub/chgnet/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 [![arXiv](https://img.shields.io/badge/arXiv-2302.14231-blue)](https://arxiv.org/abs/2302.14231)
 ![GitHub repo size](https://img.shields.io/github/repo-size/CederGroupHub/chgnet)
 [![PyPI](https://img.shields.io/pypi/v/chgnet?logo=pypi&logoColor=white)](https://pypi.org/project/chgnet?logo=pypi&logoColor=white)
+
 </h4>
 
 A pretrained universal neural network potential for
 **charge**-informed atomistic modeling
 ![chgnet](chgnet-logo.png)
 **C**rystal **H**amiltonian **G**raph neural **Net**work is pretrained on the GGA/GGA+U static and relaxation trajectories from Materials Project,
 a comprehensive dataset consisting of 1.5 Million structures from 146k compounds spanning the whole periodic table.
@@ -44,29 +45,28 @@
 in atomistic modeling with near DFT accuracy. The charge inference is realized by regularizing the atom features with
 DFT magnetic moments, which carry rich information about both local ionic environments and charge distribution.
 
 ## Example notebooks
 
 | Notebooks                                                                                                                | Links&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;                                                                                                     | Descriptions                                                                                                                        |
 | ------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
-| [**Using CHGNet**](https://github.com/CederGroupHub/chgnet/blob/main/examples/CHGNet_examples.ipynb)                     | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/CHGNet_examples.ipynb)             | Examples for loading pre-trained CHGNet, predicting energy, force, stress, magmom as well as running structure optimization and MD. |
+| [**CHGNet Basics**](https://github.com/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)                     | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)             | Examples for loading pre-trained CHGNet, predicting energy, force, stress, magmom as well as running structure optimization and MD. |
 | [**Tuning CHGNet**](https://github.com/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                        | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                 | Examples of fine tuning the pretrained CHGNet to your system of interest.                                                           |
 | [**Visualize Relaxation**](https://github.com/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | Crystal Toolkit that visualizes atom positions, energies and forces of a structure during CHGNet relaxation.                        |
 
 [Open in Google Colab]: https://colab.research.google.com/assets/colab-badge.svg
 
 ## Installation
 
 You can install `chgnet` through `pip`:
 
 ```sh
 pip install chgnet
 ```
 
-
 ## Usage
 
 ### Direct Inference (Static Calculation)
 
 Pretrained `CHGNet` can predict the energy (eV/atom), force (eV/A), stress (GPa) and
 magmom ($\mu_B$) of a given structure.
 
@@ -109,15 +109,15 @@
 ```
 
 Visualize the magnetic moments after the MD run
 
 ```python
 from ase.io.trajectory import Trajectory
 from pymatgen.io.ase import AseAtomsAdaptor
-from chgnet.utils.utils import solve_charge_by_mag
+from chgnet.utils import solve_charge_by_mag
 
 traj = Trajectory("md_out.traj")
 mag = traj[-1].get_magnetic_moments()
 
 # get the non-charge-decorated structure
 structure = AseAtomsAdaptor.get_structure(traj[-1])
 print(structure)
```

### Comparing `chgnet-0.1.3/README.md` & `chgnet-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 [![Tests](https://github.com/CederGroupHub/chgnet/actions/workflows/test.yml/badge.svg)](https://github.com/CederGroupHub/chgnet/actions/workflows/test.yml)
 [![Linting](https://github.com/CederGroupHub/chgnet/actions/workflows/lint.yml/badge.svg)](https://github.com/CederGroupHub/chgnet/actions/workflows/lint.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/e3bdcea0382a495d96408e4f84408e85)](https://app.codacy.com/gh/CederGroupHub/chgnet/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 [![arXiv](https://img.shields.io/badge/arXiv-2302.14231-blue)](https://arxiv.org/abs/2302.14231)
 ![GitHub repo size](https://img.shields.io/github/repo-size/CederGroupHub/chgnet)
 [![PyPI](https://img.shields.io/pypi/v/chgnet?logo=pypi&logoColor=white)](https://pypi.org/project/chgnet?logo=pypi&logoColor=white)
+
 </h4>
 
 A pretrained universal neural network potential for
 **charge**-informed atomistic modeling
 ![chgnet](chgnet-logo.png)
 **C**rystal **H**amiltonian **G**raph neural **Net**work is pretrained on the GGA/GGA+U static and relaxation trajectories from Materials Project,
 a comprehensive dataset consisting of 1.5 Million structures from 146k compounds spanning the whole periodic table.
@@ -20,29 +21,28 @@
 in atomistic modeling with near DFT accuracy. The charge inference is realized by regularizing the atom features with
 DFT magnetic moments, which carry rich information about both local ionic environments and charge distribution.
 
 ## Example notebooks
 
 | Notebooks                                                                                                                | Links&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;                                                                                                     | Descriptions                                                                                                                        |
 | ------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
-| [**Using CHGNet**](https://github.com/CederGroupHub/chgnet/blob/main/examples/CHGNet_examples.ipynb)                     | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/CHGNet_examples.ipynb)             | Examples for loading pre-trained CHGNet, predicting energy, force, stress, magmom as well as running structure optimization and MD. |
+| [**CHGNet Basics**](https://github.com/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)                     | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)             | Examples for loading pre-trained CHGNet, predicting energy, force, stress, magmom as well as running structure optimization and MD. |
 | [**Tuning CHGNet**](https://github.com/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                        | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                 | Examples of fine tuning the pretrained CHGNet to your system of interest.                                                           |
 | [**Visualize Relaxation**](https://github.com/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | Crystal Toolkit that visualizes atom positions, energies and forces of a structure during CHGNet relaxation.                        |
 
 [Open in Google Colab]: https://colab.research.google.com/assets/colab-badge.svg
 
 ## Installation
 
 You can install `chgnet` through `pip`:
 
 ```sh
 pip install chgnet
 ```
 
-
 ## Usage
 
 ### Direct Inference (Static Calculation)
 
 Pretrained `CHGNet` can predict the energy (eV/atom), force (eV/A), stress (GPa) and
 magmom ($\mu_B$) of a given structure.
 
@@ -85,15 +85,15 @@
 ```
 
 Visualize the magnetic moments after the MD run
 
 ```python
 from ase.io.trajectory import Trajectory
 from pymatgen.io.ase import AseAtomsAdaptor
-from chgnet.utils.utils import solve_charge_by_mag
+from chgnet.utils import solve_charge_by_mag
 
 traj = Trajectory("md_out.traj")
 mag = traj[-1].get_magnetic_moments()
 
 # get the non-charge-decorated structure
 structure = AseAtomsAdaptor.get_structure(traj[-1])
 print(structure)
```

### Comparing `chgnet-0.1.3/chgnet/data/dataset.py` & `chgnet-0.1.4/chgnet/data/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 from torch.utils.data import DataLoader, Dataset
 from torch.utils.data.sampler import SubsetRandomSampler
 
 from chgnet import utils
 from chgnet.graph import CrystalGraph, CrystalGraphConverter
 
 if TYPE_CHECKING:
-    from chgnet import PredTask, TrainTask
+    from chgnet import TrainTask
 
 warnings.filterwarnings("ignore")
 datatype = torch.float32
 
 
 class StructureData(Dataset):
     """A simple torch Dataset of structures."""
 
     def __init__(
         self,
         structures: list[Structure],
         energies: list[float],
         forces: list[Sequence[Sequence[float]]],
-        stresses: list[Sequence[Sequence[float]]] = None,
-        magmoms: list[Sequence[Sequence[float]]] = None,
-        graph_converter: CrystalGraphConverter = None,
+        stresses: list[Sequence[Sequence[float]]] | None | None = None,
+        magmoms: list[Sequence[Sequence[float]]] | None | None = None,
+        graph_converter: CrystalGraphConverter | None | None = None,
     ) -> None:
         """Initialize the dataset.
 
         Args:
             structures (list[dict]): pymatgen Structure objects.
             energies (list[float]): [data_size, 1]
             forces (list[list[float]]): [data_size, n_atoms, 3]
@@ -119,41 +119,53 @@
 class CIFData(Dataset):
     """A dataset from CIFs."""
 
     def __init__(
         self,
         cif_path: str,
         labels: str | dict = "labels.json",
-        targets: TrainTask = "ef",
-        graph_converter: CrystalGraphConverter = None,
-        energy_str: str = "energy_per_atom",
+        targets: TrainTask = "efsm",
+        graph_converter: CrystalGraphConverter | None = None,
+        energy_key: str = "energy_per_atom",
+        force_key: str = "force",
+        stress_key: str = "stress",
+        magmom_key: str = "magmom",
     ) -> None:
         """Initialize the dataset from a directory containing CIFs.
 
         Args:
             cif_path (str): path that contain all the graphs, labels.json
             labels (str, dict): the path or dictionary of labels
-            targets ('ef' | 'efs' | 'efsm'): the training targets e=energy, f=forces,
-                s=stress, m=magmons. Default = "ef"
+            targets ("ef" | "efs" | "efm" | "efsm"): The training targets.
+                Default = "efsm"
             graph_converter (CrystalGraphConverter, optional):
                 a CrystalGraphConverter to convert the structures,
                 if None, it will be set to CHGNet default converter
-            energy_str (str, optional): the key of energy in the labels.
+            energy_key (str, optional): the key of energy in the labels.
                 Default = "energy_per_atom".
+            force_key (str, optional): the key of force in the labels.
+                Default = "force".
+            stress_key (str, optional): the key of stress in the labels.
+                Default = "stress".
+            magmom_key (str, optional): the key of magmom in the labels.
+                Default = "magmom".
         """
         self.data_dir = cif_path
         self.data = utils.read_json(os.path.join(cif_path, labels))
         self.cif_ids = list(self.data)
         random.shuffle(self.cif_ids)
         print(f"{cif_path}: {len(self.cif_ids):,} structures imported")
         self.graph_converter = graph_converter or CrystalGraphConverter(
             atom_graph_cutoff=5, bond_graph_cutoff=3
         )
 
-        self.energy_str = energy_str
+        self.energy_key = energy_key
+        self.force_key = force_key
+        self.stress_key = stress_key
+        self.magmom_key = magmom_key
         self.targets = targets
         self.failed_idx: list[int] = []
         self.failed_graph_id: dict[str, str] = {}
 
     def __len__(self) -> int:
         """Get the number of structures in this dataset."""
         return len(self.cif_ids)
@@ -175,30 +187,31 @@
                 )
                 crystal_graph = self.graph_converter(
                     structure, graph_id=graph_id, mp_id=mp_id
                 )
                 targets = {}
                 for key in self.targets:
                     if key == "e":
-                        energy = self.data[graph_id][self.energy_str]
+                        energy = self.data[graph_id][self.energy_key]
                         targets["e"] = torch.tensor(energy, dtype=datatype)
                     elif key == "f":
-                        force = self.data[graph_id]["forces"]
+                        force = self.data[graph_id][self.force_key]
                         targets["f"] = torch.tensor(force, dtype=datatype)
                     elif key == "s":
-                        stress = self.data[graph_id]["stress"]
+                        stress = self.data[graph_id][self.stress_key]
                         # Convert VASP stress
                         targets["s"] = torch.tensor(stress, dtype=datatype) * -0.1
                     elif key == "m":
-                        mag = self.data[graph_id]["magmom"]
+                        mag = self.data[graph_id][self.magmom_key]
                         # use absolute value for magnetic moments
                         targets["m"] = torch.abs(torch.tensor(mag, dtype=datatype))
                 return crystal_graph, targets
 
-            # Omit structures with isolated atoms. Return another randomly selected structure
+            # Omit structures with isolated atoms.
+            # Return another randomly selected structure
             except Exception:
                 try:
                     graph_id = self.cif_ids[idx]
                 except IndexError:
                     print(idx, len(self.cif_ids))
                 structure = Structure.from_file(
                     os.path.join(self.data_dir, f"{graph_id}.cif")
@@ -217,26 +230,39 @@
     make_graphs.py. We recommend you to use the dataset to avoid graph conversion steps.
     """
 
     def __init__(
         self,
         graph_path: str,
         labels: str | dict = "labels.json",
-        targets: PredTask = "efsm",
-        exclude: str | list | None = None,
-        energy_str: str = "energy_per_atom",
+        targets: TrainTask = "efsm",
+        exclude: str | list | None | None = None,
+        energy_key: str = "energy_per_atom",
+        force_key: str = "force",
+        stress_key: str = "stress",
+        magmom_key: str = "magmom",
     ) -> None:
         """Initialize the dataset from a directory containing saved crystal graphs.
 
         Args:
             graph_path (str): path that contain all the graphs, labels.json
-            labels (str, dict): the path or dictionary of labels
-            targets ("ef" | "efs" | "efsm"): The training targets. Default = "efsm"
-            exclude (str, list | None): the path or list of excluded graphs. Default = None
-            energy_str (str, optional): the key of energy in the labels.
+            labels (str, dict): the path or dictionary of labels.
+                Default = "labels.json"
+            targets ("ef" | "efs" | "efm" | "efsm"): The training targets.
+                Default = "efsm"
+            exclude (str, list | None): the path or list of excluded graphs.
+                Default = None
+            energy_key (str, optional): the key of energy in the labels.
+                Default = "energy_per_atom".
+            force_key (str, optional): the key of force in the labels.
+                Default = "force".
+            stress_key (str, optional): the key of stress in the labels.
+                Default = "stress".
+            magmom_key (str, optional): the key of magmom in the labels.
+                Default = "magmom".
         """
         self.graph_path = graph_path
         if isinstance(labels, str):
             labels = os.path.join(graph_path, labels)
             print(f"Importing: {labels}")
             self.labels = utils.read_json(labels)
         elif isinstance(labels, dict):
@@ -247,25 +273,28 @@
         elif isinstance(exclude, list):
             self.excluded_graph = exclude
         else:
             self.excluded_graph = []
 
         self.keys = []
         for mp_id, dic in self.labels.items():
-            for graph_id, _ in dic.items():
+            for graph_id in dic:
                 self.keys.append((mp_id, graph_id))
         random.shuffle(self.keys)
         print(f"{len(self.labels)} mp_ids, {len(self)} frames imported")
         if self.excluded_graph is not None:
             print(f"{len(self.excluded_graph)} graphs are pre-excluded")
 
-        self.energy_str = energy_str
+        self.energy_key = energy_key
+        self.force_key = force_key
+        self.stress_key = stress_key
+        self.magmom_key = magmom_key
         self.targets = targets
         self.failed_idx: list[int] = []
-        self.failed_graph_id: dict[str, str] = {}
+        self.failed_graph_id: list[str] = []
 
     def __len__(self) -> int:
         """Get the number of graphs in this dataset."""
         return len(self.keys)
 
     def __getitem__(self, idx) -> tuple[CrystalGraph, dict[str, Tensor]]:
         """Get one item in the dataset.
@@ -283,25 +312,25 @@
                 return self.__getitem__(idx)
             try:
                 graph_path = os.path.join(self.graph_path, f"{graph_id}.pt")
                 crystal_graph = CrystalGraph.from_file(graph_path)
                 targets = {}
                 for key in self.targets:
                     if key == "e":
-                        energy = self.labels[mp_id][graph_id][self.energy_str]
+                        energy = self.labels[mp_id][graph_id][self.energy_key]
                         targets["e"] = torch.tensor(energy, dtype=datatype)
-                    elif key == "f" or key == "force":
-                        force = self.labels[mp_id][graph_id]["force"]
+                    elif key == "f":
+                        force = self.labels[mp_id][graph_id][self.force_key]
                         targets["f"] = torch.tensor(force, dtype=datatype)
-                    elif key == "s" or key == "stresses":
-                        stress = self.labels[mp_id][graph_id]["stress"]
+                    elif key == "s":
+                        stress = self.labels[mp_id][graph_id][self.magmom_key]
                         # Convert VASP stress
                         targets["s"] = torch.tensor(stress, dtype=datatype) * (-0.1)
                     elif key == "m":
-                        mag = self.labels[mp_id][graph_id]["magmom"]
+                        mag = self.labels[mp_id][graph_id][self.magmom_key]
                         # use absolute value for magnetic moments
                         if mag is None:
                             targets["m"] = None
                         else:
                             targets["m"] = torch.abs(torch.tensor(mag, dtype=datatype))
                 return crystal_graph, targets
 
@@ -315,17 +344,17 @@
             idx = random.randint(0, len(self) - 1)
             return self.__getitem__(idx)
 
     def get_train_val_test_loader(
         self,
         train_ratio: float = 0.8,
         val_ratio: float = 0.1,
-        train_key: list[str] = None,
-        val_key: list[str] = None,
-        test_key: list[str] = None,
+        train_key: list[str] | None | None = None,
+        val_key: list[str] | None | None = None,
+        test_key: list[str] | None | None = None,
         batch_size=32,
         num_workers=0,
         pin_memory=True,
     ) -> tuple[DataLoader, DataLoader, DataLoader]:
         """Partition the GraphData using materials id,
         randomly select the train_keys, val_keys, test_keys by train val test ratio,
         or use pre-defined train_keys, val_keys, and test_keys to create train, val,
@@ -434,24 +463,35 @@
     """
 
     def __init__(
         self,
         data: str | dict,
         graph_converter: CrystalGraphConverter,
         targets: TrainTask = "efsm",
-        energy_str: str = "energy_per_atom",
+        energy_key: str = "energy_per_atom",
+        force_key: str = "force",
+        stress_key: str = "stress",
+        magmom_key: str = "magmom",
     ) -> None:
         """Initialize the dataset by reading Json files.
 
         Args:
             data (str | dict): file path or dir name that contain all the JSONs
             graph_converter (CrystalGraphConverter): Converts pymatgen.core.Structure to graph
-            targets ('ef' | 'efs' | 'efsm'): the training targets e=energy, f=forces, s=stress,
-                m=magmons. Default = "efsm".
-            energy_str (str): key to get energy from the JSON file. Default = "energy_per_atom"
+            targets ("ef" | "efs" | "efm" | "efsm"): The training targets.
+                Default = "efsm"
+            energy_key (str, optional): the key of energy in the labels.
+                Default = "energy_per_atom".
+            force_key (str, optional): the key of force in the labels.
+                Default = "force".
+            stress_key (str, optional): the key of stress in the labels.
+                Default = "stress".
+            magmom_key (str, optional): the key of magmom in the labels.
+                Default = "magmom".
+
         """
         if isinstance(data, str):
             self.data = {}
             if os.path.isdir(data):
                 for json_path in os.listdir(data):
                     if json_path.endswith(".json"):
                         print(f"Importing: {json_path}")
@@ -467,15 +507,18 @@
         self.keys = []
         for mp_id, dic in self.data.items():
             for graph_id in dic:
                 self.keys.append((mp_id, graph_id))
         random.shuffle(self.keys)
         print(f"{len(self.data)} mp_ids, {len(self)} structures imported")
         self.graph_converter = graph_converter
-        self.energy_str = energy_str
+        self.energy_key = energy_key
+        self.force_key = force_key
+        self.stress_key = stress_key
+        self.magmom_key = magmom_key
         self.targets = targets
         self.failed_idx: list[int] = []
         self.failed_graph_id: dict[str, str] = {}
 
     def __len__(self) -> int:
         """Get the number of structures with targets in the dataset."""
         return len(self.keys)
@@ -495,25 +538,25 @@
                 crystal_graph = self.graph_converter(
                     struct, graph_id=graph_id, mp_id=mp_id
                 )
 
                 targets = {}
                 for key in self.targets:
                     if key == "e":
-                        energy = self.data[mp_id][graph_id][self.energy_str]
+                        energy = self.data[mp_id][graph_id][self.energy_key]
                         targets["e"] = torch.tensor(energy, dtype=datatype)
-                    elif key == "f" or key == "force":
-                        force = self.data[mp_id][graph_id]["force"]
+                    elif key == "f":
+                        force = self.data[mp_id][graph_id][self.force_key]
                         targets["f"] = torch.tensor(force, dtype=datatype)
-                    elif key == "s" or key == "stresses":
-                        stress = self.data[mp_id][graph_id]["stress"]
+                    elif key == "s":
+                        stress = self.data[mp_id][graph_id][self.stress_key]
                         # Convert VASP stress
                         targets["s"] = torch.tensor(stress, dtype=datatype) * (-0.1)
                     elif key == "m":
-                        mag = self.data[mp_id][graph_id]["magmom"]
+                        mag = self.data[mp_id][graph_id][self.magmom_key]
                         # use absolute value for magnetic moments
                         if mag is None:
                             targets["m"] = None
                         else:
                             targets["m"] = torch.abs(torch.tensor(mag, dtype=datatype))
                 return crystal_graph, targets
 
@@ -528,17 +571,17 @@
             idx = random.randint(0, len(self) - 1)
             return self.__getitem__(idx)
 
     def get_train_val_test_loader(
         self,
         train_ratio: float = 0.8,
         val_ratio: float = 0.1,
-        train_key: list[str] = None,
-        val_key: list[str] = None,
-        test_key: list[str] = None,
+        train_key: list[str] | None = None,
+        val_key: list[str] | None = None,
+        test_key: list[str] | None = None,
         batch_size=32,
         num_workers=0,
         pin_memory=True,
     ) -> tuple[DataLoader, DataLoader, DataLoader]:
         """Partition the Dataset using materials id,
         randomly select the train_keys, val_keys, test_keys by train val test ratio,
         or use pre-defined train_keys, val_keys, and test_keys to create train, val,
@@ -710,16 +753,15 @@
             batch_size=batch_size,
             collate_fn=collate_graphs,
             sampler=SubsetRandomSampler(indices=indices[train_size + val_size :]),
             num_workers=num_workers,
             pin_memory=pin_memory,
         )
         return train_loader, val_loader, test_loader
-    else:
-        return train_loader, val_loader
+    return train_loader, val_loader
 
 
 def get_loader(dataset, batch_size=64, num_workers=0, pin_memory=True):
     """Get a dataloader from a dataset.
 
     Args:
         dataset (Dataset): The dataset to partition.
@@ -730,17 +772,15 @@
             Default = 0
         pin_memory (bool): Whether to pin the memory of the data loaders
             Default: True
 
     Returns:
         data_loader
     """
-    data_loader = DataLoader(
+    return DataLoader(
         dataset,
         batch_size=batch_size,
         collate_fn=collate_graphs,
         shuffle=True,
         num_workers=num_workers,
         pin_memory=pin_memory,
     )
-
-    return data_loader
```

### Comparing `chgnet-0.1.3/chgnet/graph/converter.py` & `chgnet-0.1.4/chgnet/graph/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
 import sys
-from typing import Literal
+from typing import TYPE_CHECKING, Literal
 
 import torch
-from pymatgen.core import Structure
 from torch import Tensor, nn
 
 from chgnet.graph.crystalgraph import CrystalGraph
 from chgnet.graph.graph import Graph, Node
 
+if TYPE_CHECKING:
+    from pymatgen.core import Structure
+
 datatype = torch.float32
 
 
 class CrystalGraphConverter(nn.Module):
     """Convert a pymatgen.core.Structure to a CrystalGraph.
 
     Only the minimal essential information is kept.
@@ -100,15 +102,15 @@
         # Check if graph has isolated atom
         has_isolated_atom = not set(range(n_atoms)).issubset(center_index)
         if has_isolated_atom:
             r_cutoff = self.atom_graph_cutoff
             msg = f"{graph_id=} has isolated atom with {r_cutoff=}, should be skipped"
             if on_isolated_atoms == "ignore":
                 return None
-            elif on_isolated_atoms == "warn":
+            if on_isolated_atoms == "warn":
                 print(msg, file=sys.stderr)
                 return None
             # Discard this structure if it has isolated atom in the graph
             raise ValueError(msg)
 
         return CrystalGraph(
             atomic_number=atomic_number,
```

### Comparing `chgnet-0.1.3/chgnet/graph/crystalgraph.py` & `chgnet-0.1.4/chgnet/graph/crystalgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
         atom_graph_cutoff: float,
         neighbor_image: Tensor,
         directed2undirected: Tensor,
         undirected2directed: Tensor,
         bond_graph: Tensor,
         bond_graph_cutoff: float,
         lattice: Tensor,
-        graph_id: str = None,
-        mp_id: str = None,
-        composition: str = None,
+        graph_id: str | None = None,
+        mp_id: str | None = None,
+        composition: str | None = None,
     ) -> None:
         """Initialize the crystal graph.
         Attention! This data class is not intended to be created manually.
                    Crystal Graph should be returned by a CrystalGraphConverter
         Args:
             atomic_number (Tensor): the atomic numbers of atoms in the structure
                 [n_atom]
@@ -117,15 +117,15 @@
             "bond_graph_cutoff": self.bond_graph_cutoff,
             "lattice": self.lattice,
             "graph_id": self.graph_id,
             "mp_id": self.mp_id,
             "composition": self.composition,
         }
 
-    def save(self, fname: str = None, save_dir: str = ".") -> str:
+    def save(self, fname: str | None = None, save_dir: str = ".") -> str:
         """Save the graph to a file.
 
         Args:
             fname (str, optional): File name. Defaults to None.
             save_dir (str, optional): Directory to save the file. Defaults to ".".
 
         Returns:
@@ -146,16 +146,15 @@
 
         Args:
             file_name (str): The path to the file.
 
         Returns:
             CrystalGraph: The loaded graph.
         """
-        graph = torch.load(file_name)
-        return graph
+        return torch.load(file_name)
 
     @classmethod
     def from_dict(cls, dic: dict[str, Any]) -> CrystalGraph:
         """Load a CrystalGraph from a dictionary."""
         return CrystalGraph(**dic)
 
     def __repr__(self) -> str:
```

### Comparing `chgnet-0.1.3/chgnet/graph/graph.py` & `chgnet-0.1.4/chgnet/graph/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
-from chgnet import utils
+from chgnet.utils import write_json
 
 
 class Node:
     """A node in a graph."""
 
-    def __init__(self, index: int, info: dict = None) -> None:
+    def __init__(self, index: int, info: dict | None = None) -> None:
         """Initialize a Node.
 
         Args:
             index (int): the index of this node
             info (dict, optional): any additional information about this node.
         """
         self.index = index
@@ -28,15 +28,17 @@
         else:
             self.neighbors[index].append(edge)
 
 
 class UndirectedEdge:
     """An undirected/bi-directed edge in a graph."""
 
-    def __init__(self, nodes: list, index: int = None, info: dict = None) -> None:
+    def __init__(
+        self, nodes: list, index: int | None = None, info: dict | None = None
+    ) -> None:
         """Initialize an UndirectedEdge."""
         self.nodes = nodes
         self.index = index
         self.info = info
 
     def __repr__(self):
         """Return a string representation of this edge."""
@@ -49,15 +51,17 @@
         """Check if two undirected edges are equal."""
         return set(self.nodes) == set(other.nodes) and self.info == other.info
 
 
 class DirectedEdge:
     """A directed edge in a graph."""
 
-    def __init__(self, nodes: list, index: int = None, info: dict = None) -> None:
+    def __init__(
+        self, nodes: list, index: int | None = None, info: dict | None = None
+    ) -> None:
         """Initialize a DirectedEdge."""
         self.nodes = nodes
         self.index = index
         self.info = info
 
     def make_undirected(self, index, info=None):
         """Make a directed edge undirected."""
@@ -126,56 +130,77 @@
 
         Args:
             center_index (int): center node index
             neighbor_index (int): neighbor node index
             image (np.array): the periodic cell image the neighbor is from
             distance (float): distance between center and neighbor.
         """
+        # Create directed_edge (DE) index using the length of added DEs
         directed_edge_index = len(self.directed_edges_list)
+
+        # Create the DE with info
         this_directed_edge = DirectedEdge(
             [center_index, neighbor_index],
             index=directed_edge_index,
             info={"image": image, "distance": distance},
         )
 
+        # Record the two ends of the DE and see if they have been added
+        # Here the sequence of the ends doesn't matter since we want to
+        #  search for associated undirected_edge (UDE)
         tmp = frozenset([center_index, neighbor_index])
+
+        # This combination of two ends hasn't been added
         if tmp not in self.undirected_edges:
+            # Create UDE index
             this_directed_edge.info["undirected_edge_index"] = len(
                 self.undirected_edges_list
             )
+            # Create UDE
             this_undirected_edge = this_directed_edge.make_undirected(
                 index=len(self.undirected_edges_list),
                 info={"directed_edge_index": [directed_edge_index]},
             )
             self.undirected_edges[tmp] = [this_undirected_edge]
             self.undirected_edges_list.append(this_undirected_edge)
             self.nodes[center_index].add_neighbor(neighbor_index, this_directed_edge)
             self.directed_edges_list.append(this_directed_edge)
         else:
-            # this pair of nodes has been added before, we need to see if this time,
-            # it's the other directed edge of the same undirected edge or it's another
-            # totally different undirected edge that has different image and distance
+            # This pair of nodes has been added before, we need to see if this time,
+            # 1. it's the other directed edge of the same undirected edge or,
+            # 2. it's another totally different undirected edge that has
+            # different image and distance (this is possible consider periodicity)
             for undirected_edge in self.undirected_edges[tmp]:
                 if (
                     abs(undirected_edge.info["distance"] - distance) < 1e-6
                     and len(undirected_edge.info["directed_edge_index"]) == 1
                 ):
                     # There is an undirected edge with similar length and only one of
                     # the directed edges associated has been added
                     added_DE = self.directed_edges_list[
                         undirected_edge.info["directed_edge_index"][0]
                     ]
+
+                    # See if the DE that's associated to this UDE
+                    # is the reverse of our DE
                     if added_DE == this_directed_edge:
+                        # Add UDE index to this DE
                         this_directed_edge.info[
                             "undirected_edge_index"
                         ] = added_DE.info["undirected_edge_index"]
+
+                        # At the center node, draw edge with this DE
                         self.nodes[center_index].add_neighbor(
                             neighbor_index, this_directed_edge
                         )
+
+                        # Add this DE to DE list
                         self.directed_edges_list.append(this_directed_edge)
+
+                        # Add this DE to the UDE
                         undirected_edge.info["directed_edge_index"].append(
                             directed_edge_index
                         )
                         return
 
             # no undirected_edge matches to this directed edge
             this_directed_edge.info["undirected_edge_index"] = len(
@@ -190,23 +215,26 @@
             self.nodes[center_index].add_neighbor(neighbor_index, this_directed_edge)
             self.directed_edges_list.append(this_directed_edge)
 
     def adjacency_list(self):
         """Get the adjacency list
         Return:
             graph: the adjacency list
-                [[0, 1, 0],
-                 [0, 2, 1],
-                 ... ...  ]
+                [[0, 1],
+                 [0, 2],
+                 ...
+                 [5, 2]
+                 ...  ]]
                 the fist column specifies center/source node,
                 the second column specifies neighbor/destination node
             directed2undirected:
                 [0, 1, ...]
-                a list specifies the undirected edge index corresponding to
-                the directed edges represented in each row in the graph adjacency list.
+                a list of length = num_directed_edge that specifies
+                the undirected edge index corresponding to the directed edges
+                represented in each row in the graph adjacency list.
         """
         graph = [edge.nodes for edge in self.directed_edges_list]
         directed2undirected = [
             edge.info["undirected_edge_index"] for edge in self.directed_edges_list
         ]
         return graph, directed2undirected
 
@@ -220,77 +248,75 @@
 
         Return:
             line_graph:
                 [[0, 1, 1, 2, 2],
                 [0, 1, 1, 4, 23],
                 [1, 4, 23, 5, 66],
                 ... ...  ]
-                the fist column specifies node index at this angle,
-                the second column specifies 1st undirected edge index,
-                the third column specifies 1st directed edge index,
-                the fourth column specifies 2nd undirected edge index,
-                the fifth column specifies 2snd directed edge index,.
+                the fist column specifies node(atom) index at this angle,
+                the second column specifies 1st undirected edge(left bond) index,
+                the third column specifies 1st directed edge(left bond) index,
+                the fourth column specifies 2nd undirected edge(right bond) index,
+                the fifth column specifies 2snd directed edge(right bond) index,.
             undirected2directed:
                 [32, 45, ...]
-                a list maps the undirected edge index to one of its
-                the directed edges index
+                a list of length = num_undirected_edge that
+                maps the undirected edge index to one of its directed edges indices
         """
         assert len(self.directed_edges_list) == 2 * len(self.undirected_edges_list), (
             f"Error: number of directed edges={len(self.directed_edges_list)} != 2 * "
             f"number of undirected edges={len(self.directed_edges_list)}!"
             f"This indicates directed edges are not complete"
         )
         line_graph = []
         undirected2directed = []
+
+        # Loop through all the undirected edges(UDE)
         for u_edge in self.undirected_edges_list:
+            # Create the mapping from the UDE index to one of its DE index
             undirected2directed.append(u_edge.info["directed_edge_index"][0])
+
+            # Ignore the UDE if its length is larger than cutoff (3A for default)
             if u_edge.info["distance"] > cutoff:
                 continue
-            center1, center2 = list(u_edge.nodes)
-            try:
-                directed_edge1, directed_edge2 = u_edge.info["directed_edge_index"]
-            except ValueError:
-                print("Did not find 2 Directed_edges !!!")
-                print(u_edge)
-                print(
-                    "edge.info['directed_edge_index'] = ",
-                    u_edge.info["directed_edge_index"],
-                )
-                print()
-                print("len directed_edges_list = ", len(self.directed_edges_list))
-                print("len undirected_edges_list = ", len(self.undirected_edges_list))
-            # find directed edges starting at center1
-            for directed_edges in self.nodes[center1].neighbors.values():
-                for directed_edge in directed_edges:
-                    if directed_edge.index == directed_edge1:
-                        continue
-                    if directed_edge.info["distance"] < cutoff:
-                        line_graph.append(
-                            [
-                                center1,
-                                u_edge.index,
-                                directed_edge1,
-                                directed_edge.info["undirected_edge_index"],
-                                directed_edge.index,
-                            ]
-                        )
-            for directed_edges in self.nodes[center2].neighbors.values():
-                for directed_edge in directed_edges:
-                    if directed_edge.index == directed_edge2:
-                        continue
-                    if directed_edge.info["distance"] < cutoff:
-                        line_graph.append(
-                            [
-                                center2,
-                                u_edge.index,
-                                directed_edge2,
-                                directed_edge.info["undirected_edge_index"],
-                                directed_edge.index,
-                            ]
-                        )
+
+            # Assert if the UDE is valid
+            # if encountered exception,
+            # it means after Atom_Graph creation, the UDE has only 1 DE associated
+            # This exception is not encountered from the develop team's experience
+            assert len(u_edge.info["directed_edge_index"]) == 2, (
+                "Did not find 2 Directed_edges !!!"
+                f"undirected edge {u_edge} has:"
+                f"edge.info['directed_edge_index'] = "
+                f"{u_edge.info['directed_edge_index']}"
+                f"len directed_edges_list = {len(self.directed_edges_list)}"
+                f"len undirected_edges_list = {len(self.undirected_edges_list)}"
+            )
+
+            # This UDE is valid to be considered as a node in Bond_Graph
+
+            # Get the two ends (centers) and the two DE associated with this UDE
+            # DE1 should have center=center1 and DE2 should have center=center2
+            # We will need to find directed edges with center = center1
+            # and create angles with DE1, then do the same for center2 and DE2
+            for center, DE in zip(u_edge.nodes, u_edge.info["directed_edge_index"]):
+                for directed_edges in self.nodes[center].neighbors.values():
+                    for directed_edge in directed_edges:
+                        if directed_edge.index == DE:
+                            continue
+                        if directed_edge.info["distance"] < cutoff:
+                            line_graph.append(
+                                [
+                                    center,
+                                    u_edge.index,
+                                    DE,
+                                    directed_edge.info["undirected_edge_index"],
+                                    directed_edge.index,
+                                ]
+                            )
         return line_graph, undirected2directed
 
     def undirected2directed(self):
         """The index map from undirected_edge index to one of its directed_edge
         index.
         """
         out = []
@@ -306,16 +332,15 @@
             "directed_edges_list": self.directed_edges_list,
             "undirected_edges": self.undirected_edges,
             "undirected_edges_list": self.undirected_edges_list,
         }
 
     def to(self, filename="graph.json"):
         """Save graph dictionary to file."""
-        utils.write_json(self.as_dict(), filename)
-        return
+        write_json(self.as_dict(), filename)
 
     def __repr__(self) -> str:
         """Return string representation of the Graph."""
         num_nodes = len(self.nodes)
         num_directed_edges = len(self.directed_edges_list)
         num_undirected_edges = len(self.undirected_edges_list)
         return f"Graph({num_nodes=}, {num_directed_edges=}, {num_undirected_edges=})"
```

### Comparing `chgnet-0.1.3/chgnet/model/basis.py` & `chgnet-0.1.4/chgnet/model/basis.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,19 @@
 
 class GaussianExpansion(nn.Module):
     """Expands the distance by Gaussian basis.
     Unit: angstrom.
     """
 
     def __init__(
-        self, min: float = 0, max: float = 5, step: float = 0.5, var: float = None
+        self,
+        min: float = 0,
+        max: float = 5,
+        step: float = 0.5,
+        var: float | None = None,
     ) -> None:
         """Gaussian Expansion
         expand a scalar feature to a soft-one-hot feature vector.
 
         Args:
             min (float): minimum Gaussian center value
             max (float): maximum Gaussian center value
@@ -192,9 +196,8 @@
             env_val = (
                 1
                 + self.a * r_scaled**self.p
                 + self.b * r_scaled ** (self.p + 1)
                 + self.c * r_scaled ** (self.p + 2)
             )
             return torch.where(r_scaled < 1, env_val, torch.zeros_like(r_scaled))
-        else:
-            return r.new_ones(r.shape)
+        return r.new_ones(r.shape)
```

### Comparing `chgnet-0.1.3/chgnet/model/composition_model.py` & `chgnet-0.1.4/chgnet/model/composition_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 import collections
-from typing import Sequence
+from typing import TYPE_CHECKING, Sequence
 
 import numpy as np
 import torch
 from pymatgen.core import Structure
 from torch import Tensor, nn
 
-from chgnet.graph.crystalgraph import CrystalGraph
 from chgnet.model.functions import GatedMLP, find_activation
 
+if TYPE_CHECKING:
+    from chgnet.graph.crystalgraph import CrystalGraph
+
 
 class CompositionModel(nn.Module):
     """A simple FC model that takes in a chemical composition (no structure info)
     and outputs energy.
     """
 
     def __init__(
```

### Comparing `chgnet-0.1.3/chgnet/model/dynamics.py` & `chgnet-0.1.4/chgnet/model/dynamics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from __future__ import annotations
 
 import contextlib
 import io
 import pickle
 import sys
+from typing import TYPE_CHECKING
 
 import numpy as np
 import torch
 from ase import Atoms, units
 from ase.calculators.calculator import Calculator, all_changes, all_properties
 from ase.constraints import ExpCellFilter
-from ase.io import Trajectory
 from ase.md.nptberendsen import Inhomogeneous_NPTBerendsen, NPTBerendsen
 from ase.md.nvtberendsen import NVTBerendsen
 from ase.optimize.bfgs import BFGS
 from ase.optimize.bfgslinesearch import BFGSLineSearch
 from ase.optimize.fire import FIRE
 from ase.optimize.lbfgs import LBFGS, LBFGSLineSearch
 from ase.optimize.mdmin import MDMin
-from ase.optimize.optimize import Optimizer
 from ase.optimize.sciopt import SciPyFminBFGS, SciPyFminCG
 from pymatgen.analysis.eos import BirchMurnaghan
 from pymatgen.core.structure import Molecule, Structure
 from pymatgen.io.ase import AseAtomsAdaptor
 
 from chgnet.model.model import CHGNet
 
+if TYPE_CHECKING:
+    from ase.io import Trajectory
+    from ase.optimize.optimize import Optimizer
+
 # We would like to thank M3GNet develop team for this module
 # source: https://github.com/materialsvirtuallab/m3gnet
 
 OPTIMIZERS = {
     "FIRE": FIRE,
     "BFGS": BFGS,
     "LBFGS": LBFGS,
@@ -40,15 +43,15 @@
     "BFGSLineSearch": BFGSLineSearch,
 }
 
 
 class CHGNetCalculator(Calculator):
     """CHGNet Calculator for ASE applications."""
 
-    implemented_properties = ["energy", "forces", "stress", "magmoms"]
+    implemented_properties = ("energy", "forces", "stress", "magmoms")
 
     def __init__(
         self,
         model: CHGNet | None = None,
         use_device: str | None = None,
         stress_weight: float | None = 1 / 160.21766208,
         **kwargs,
@@ -80,32 +83,32 @@
         self.model = model.to(self.device)
         self.stress_weight = stress_weight
         print(f"CHGNet will run on {self.device}")
 
     def calculate(
         self,
         atoms: Atoms | None = None,
-        desired_properties: list | None = None,
-        changed_properties: list | None = None,
+        properties: list | None = None,
+        system_changes: list | None = None,
     ) -> None:
         """Calculate various properties of the atoms using CHGNet.
 
         Args:
             atoms (Atoms | None): The atoms object to calculate properties for.
-            desired_properties (list | None): The properties to calculate.
+            properties (list | None): The properties to calculate.
                 Default is all properties.
-            changed_properties (list | None): The changes made to the system.
+            system_changes (list | None): The changes made to the system.
                 Default is all changes.
         """
-        desired_properties = desired_properties or all_properties
-        changed_properties = changed_properties or all_changes
+        properties = properties or all_properties
+        system_changes = system_changes or all_changes
         super().calculate(
             atoms=atoms,
-            properties=desired_properties,
-            system_changes=changed_properties,
+            properties=properties,
+            system_changes=system_changes,
         )
 
         # Run CHGNet
         structure = AseAtomsAdaptor.get_structure(atoms)
         graph = self.model.graph_converter(structure)
         model_prediction = self.model.predict_graph(graph.to(self.device), task="efsm")
 
@@ -121,17 +124,17 @@
 
 
 class StructOptimizer:
     """Wrapper class for structural relaxation."""
 
     def __init__(
         self,
-        model: CHGNet = None,
+        model: CHGNet | None = None,
         optimizer_class: Optimizer | str | None = "FIRE",
-        use_device: str = None,
+        use_device: str | None = None,
         stress_weight: float = 1 / 160.21766208,
     ) -> None:
         """Provide a trained CHGNet model and an optimizer to relax crystal structures.
 
         Args:
             model (CHGNet): instance of a chgnet model
             optimizer_class (Optimizer,str): choose optimizer from ASE.
@@ -246,21 +249,20 @@
         self.cells.append(self.atoms.get_cell()[:])
 
     def __len__(self) -> int:
         """The number of steps in the trajectory."""
         return len(self.energies)
 
     def compute_energy(self) -> float:
-        """Calculate the energy, here we just use the potential energy.
+        """Calculate the potential energy.
 
         Returns:
             energy (float): the potential energy.
         """
-        energy = self.atoms.get_potential_energy()
-        return energy
+        return self.atoms.get_potential_energy()
 
     def save(self, filename: str) -> None:
         """Save the trajectory to file.
 
         Args:
             filename (str): filename to save the trajectory
         """
@@ -279,27 +281,27 @@
 
 class MolecularDynamics:
     """Molecular dynamics class."""
 
     def __init__(
         self,
         atoms: Atoms | Structure,
-        model: CHGNet = None,
+        model: CHGNet | None = None,
         ensemble: str = "nvt",
         temperature: int = 300,
         timestep: float = 2.0,
         pressure: float = 1.01325 * units.bar,
         taut: float | None = None,
         taup: float | None = None,
         compressibility_au: float | None = None,
         trajectory: str | Trajectory | None = None,
         logfile: str | None = None,
         loginterval: int = 1,
         append_trajectory: bool = False,
-        use_device: str = None,
+        use_device: str | None = None,
     ) -> None:
         """Initialize the MD class.
 
         Args:
             atoms (Atoms): atoms to run the MD
             model (CHGNet): model
             ensemble (str): choose from 'nvt' or 'npt'
@@ -439,17 +441,17 @@
 
 
 class EquationOfState:
     """Class to calculate equation of state."""
 
     def __init__(
         self,
-        model: CHGNet = None,
+        model: CHGNet | None = None,
         optimizer_class: Optimizer | str | None = "FIRE",
-        use_device: str = None,
+        use_device: str | None = None,
         stress_weight: float = 1 / 160.21766208,
     ) -> None:
         """Initialize a structure optimizer object for calculation of bulk modulus.
 
         Args:
             model (CHGNet): instance of a chgnet model
             optimizer_class (Optimizer,str): choose optimizer from ASE.
@@ -518,41 +520,37 @@
                 Default = "eV/A^3"
 
         Returns:
             Bulk Modulus (float)
         """
         if self.fitted is False:
             raise ValueError(
-                "Equation of state needs to be fitted " "first through self.fit()"
+                "Equation of state needs to be fitted first through self.fit()"
             )
         if unit == "eV/A^3":
             return self.bm.b0
-        elif unit == "GPa":
+        if unit == "GPa":
             return self.bm.b0_GPa
-        else:
-            raise NotImplementedError("unit has to be eV/A^3 or GPa")
+        raise NotImplementedError("unit has to be eV/A^3 or GPa")
 
     def get_compressibility(self, unit: str = "A^3/eV"):
         """Get the bulk modulus of from the fitted Birch-Murnaghan equation of state.
 
         Args:
             unit (str): The unit of bulk modulus. Can be "A^3/eV",
             "GPa^-1" "Pa^-1" or "m^2/N"
                 Default = "A^3/eV"
 
         Returns:
             Bulk Modulus (float)
         """
         if self.fitted is False:
             raise ValueError(
-                "Equation of state needs to be fitted " "first through self.fit()"
+                "Equation of state needs to be fitted first through self.fit()"
             )
         if unit == "A^3/eV":
             return 1 / self.bm.b0
-        elif unit == "GPa^-1":
+        if unit == "GPa^-1":
             return 1 / self.bm.b0_GPa
-        elif unit in ["Pa^-1", "m^2/N"]:
+        if unit in ["Pa^-1", "m^2/N"]:
             return 1 / (self.bm.b0_GPa * 1e9)
-        else:
-            raise NotImplementedError(
-                "unit has to be one of A^3/eV, " "GPa^-1 Pa^-1 or m^2/N"
-            )
+        raise NotImplementedError("unit has to be one of A^3/eV, GPa^-1 Pa^-1 or m^2/N")
```

### Comparing `chgnet-0.1.3/chgnet/model/encoders.py` & `chgnet-0.1.4/chgnet/model/encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,9 +135,8 @@
 
         Returns:
             angle_fea (Tensor):  expanded cos_ij [n_angle, angle_feature_dim]
         """
         # 1 - 1e-6 for torch.acos stability
         cosine_ij = torch.sum(bond_i * bond_j, dim=1) * (1 - 1e-6)
         angle = torch.acos(cosine_ij)
-        result = self.fourier_expansion(angle)
-        return result
+        return self.fourier_expansion(angle)
```

### Comparing `chgnet-0.1.3/chgnet/model/functions.py` & `chgnet-0.1.4/chgnet/model/functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
 
 class MLP(nn.Module):
     """Multi-Layer Perceptron used for non-linear regression."""
 
     def __init__(
         self,
-        input_dim: int = None,
-        output_dim: int | None = 1,
+        input_dim: int,
+        output_dim: int = 1,
         hidden_dim: int | Sequence[int] | None = (64, 64),
         dropout: float = 0,
         activation: str = "silu",
     ) -> None:
         """Initialize the MLP.
 
         Args:
@@ -69,22 +69,26 @@
         elif type(hidden_dim) == int:
             layers = [
                 nn.Linear(input_dim, hidden_dim),
                 find_activation(activation),
                 nn.Dropout(dropout),
                 nn.Linear(hidden_dim, output_dim),
             ]
-        else:  # type(hidden_dim) == list:
+        elif isinstance(hidden_dim, Sequence):
             layers = [nn.Linear(input_dim, hidden_dim[0]), find_activation(activation)]
             if len(hidden_dim) != 1:
                 for h_in, h_out in zip(hidden_dim[0:-1], hidden_dim[1:]):
                     layers.append(nn.Linear(h_in, h_out))
                     layers.append(find_activation(activation))
             layers.append(nn.Dropout(dropout))
             layers.append(nn.Linear(hidden_dim[-1], output_dim))
+        else:
+            raise TypeError(
+                f"{hidden_dim=} must be an integer, a list of integers, or None."
+            )
         self.layers = nn.Sequential(*layers)
 
     def forward(self, X: Tensor) -> Tensor:
         """Performs a forward pass through the MLP.
 
         Args:
             X (Tensor): a tensor of shape (batch_size, input_dim)
@@ -98,16 +102,16 @@
 class GatedMLP(nn.Module):
     """Gated MLP
     similar model structure is used in CGCNN and M3GNet.
     """
 
     def __init__(
         self,
-        input_dim: int = None,
-        output_dim: int = None,
+        input_dim: int,
+        output_dim: int,
         hidden_dim: int | list[int] | None = None,
         dropout=0,
         activation="silu",
         norm="batch",
     ) -> None:
         """Initialize a gated MLP.
 
@@ -187,15 +191,15 @@
             "sigmoid": nn.Sigmoid,
             "tanh": nn.Tanh,
         }[name.lower()]()
     except KeyError as exc:
         raise NotImplementedError from exc
 
 
-def find_normalization(name: str, dim: int = None) -> nn.Module | None:
+def find_normalization(name: str, dim: int | None = None) -> nn.Module | None:
     """Return an normalization function using name."""
     if name is None:
         return None
     return {
         "batch": nn.BatchNorm1d(dim),
         "layer": nn.LayerNorm(dim),
     }.get(name.lower(), None)
```

### Comparing `chgnet-0.1.3/chgnet/model/layers.py` & `chgnet-0.1.4/chgnet/model/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def __init__(
         self,
         atom_fea_dim: int,
         bond_fea_dim: int,
         hidden_dim: int = 64,
         dropout: float = 0,
         activation: str = "silu",
-        norm: str = None,
+        norm: str | None = None,
         use_mlp_out: bool = True,
         resnet: bool = True,
         gMLP_norm: str = "batch",
     ) -> None:
         """Args:
         atom_fea_dim (int): The dimensionality of the input atom features.
         bond_fea_dim (int): The dimensionality of the input bond features.
@@ -133,15 +133,15 @@
         self,
         atom_fea_dim: int,
         bond_fea_dim: int,
         angle_fea_dim: int,
         hidden_dim: int = 64,
         dropout: float = 0,
         activation: str = "silu",
-        norm: str = None,
+        norm: str | None = None,
         use_mlp_out: bool = True,
         resnet=True,
         **kwargs,
     ) -> None:
         """Args:
         atom_fea_dim (int): The dimensionality of the input atom features.
         bond_fea_dim (int): The dimensionality of the input bond features.
@@ -200,15 +200,15 @@
             bond_feas (Tensor): bond features tensor with shape
                 [num_undirected_bonds, bond_fea_dim]
             bond_weights (Tensor): BondGraph bond weights with shape
                 [num_undirected_bonds, bond_fea_dim]
             angle_feas (Tensor): angle features tensor with shape
                 [num_batch_angles, atom_fea_dim]
             bond_graph (Tensor): Directed BondGraph tensor with shape
-                [num_batched_angles, 5]
+                [num_batched_angles, 3]
 
         Returns:
             new_bond_feas (Tensor): bond feature tensor with shape
                 [num_batch_atom, bond_fea_dim]
 
         Notes:
             - num_batch_atoms = sum(num_atoms) in batch
@@ -251,15 +251,15 @@
         self,
         atom_fea_dim: int,
         bond_fea_dim: int,
         angle_fea_dim: int,
         hidden_dim: int = 0,
         dropout: float = 0,
         activation: str = "silu",
-        norm: str = None,
+        norm: str | None = None,
         resnet: bool = True,
         **kwargs,
     ) -> None:
         """Create a new AngleUpdate instance.
 
         Args:
             atom_fea_dim (int): The dimensionality of the input atom features.
@@ -308,15 +308,15 @@
             atom_feas (Tensor): atom features tensor with shape
                 [num_batch_atoms, atom_fea_dim]
             bond_feas (Tensor): bond features tensor with shape
                 [num_undirected_bonds, bond_fea_dim]
             angle_feas (Tensor): angle features tensor with shape
                 [num_batch_angles, atom_fea_dim]
             bond_graph (Tensor): Directed BondGraph tensor with shape
-                [num_batched_angles, 5]
+                [num_batched_angles, 3]
 
         Returns:
             new_angle_feas (Tensor): angle features tensor with shape
                 [num_batch_angles, atom_fea_dim]
 
         Notes:
             - num_batch_atoms = sum(num_atoms) in batch
```

### Comparing `chgnet-0.1.3/chgnet/model/model.py` & `chgnet-0.1.4/chgnet/model/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,32 +32,33 @@
     """
 
     def __init__(
         self,
         atom_fea_dim: int = 64,
         bond_fea_dim: int = 64,
         angle_fea_dim: int = 64,
-        composition_model: str | nn.Module = None,
+        composition_model: str | nn.Module = "MPtrj",
         num_radial: int = 9,
         num_angular: int = 9,
         n_conv: int = 4,
         atom_conv_hidden_dim: Sequence[int] | int = 64,
         update_bond: bool = True,
         bond_conv_hidden_dim: Sequence[int] | int = 64,
         update_angle: bool = True,
         angle_layer_hidden_dim: Sequence[int] | int = 0,
         conv_dropout: float = 0,
         read_out: str = "ave",
         mlp_hidden_dims: Sequence[int] | int = (64, 64),
         mlp_dropout: float = 0,
         mlp_first: bool = True,
         is_intensive: bool = True,
-        non_linearity: Literal["silu", "relu", "tanh", "gelu"] = "relu",
+        non_linearity: Literal["silu", "relu", "tanh", "gelu"] = "silu",
         atom_graph_cutoff: int = 5,
         bond_graph_cutoff: int = 3,
+        cutoff_coeff: int = 5,
         learnable_rbf: bool = True,
         **kwargs,
     ) -> None:
         """Initialize the CHGNet.
 
         Args:
             atom_fea_dim (int): atom feature vector embedding dimension.
@@ -113,14 +114,15 @@
             atom_graph_cutoff (float): cutoff radius (A) in creating atom_graph,
                 this need to be consistent with the value in training dataloader
                 Default = 5
             bond_graph_cutoff (float): cutoff radius (A) in creating bond_graph,
                 this need to be consistent with value in training dataloader
                 Default = 3
             cutoff_coeff (float): cutoff strength used in graph smooth cutoff function.
+                the smaller this coeff is, the smoother the basis is
                 Default = 5
             learnable_rbf (bool): whether to set the frequencies in rbf and Fourier
                 basis functions learnable.
                 Default = True
             **kwargs: Additional keyword arguments
         """
         # Store model args for reconstruction
@@ -136,31 +138,32 @@
         self.bond_fea_dim = bond_fea_dim
         self.is_intensive = is_intensive
         self.n_conv = n_conv
 
         # Optionally, define composition model
         if isinstance(composition_model, nn.Module):
             self.composition_model = composition_model
-        else:
+        elif isinstance(composition_model, str):
             self.composition_model = AtomRef(is_intensive=is_intensive)
-            if isinstance(composition_model, str):
-                self.composition_model.initialize_from(composition_model)
+            self.composition_model.initialize_from(composition_model)
+        else:
+            self.composition_model = None
+
         if self.composition_model is not None:
             # fixed composition_model weights
             for param in self.composition_model.parameters():
                 param.requires_grad = False
 
         # Define Crystal Graph Converter
         self.graph_converter = CrystalGraphConverter(
             atom_graph_cutoff=atom_graph_cutoff, bond_graph_cutoff=bond_graph_cutoff
         )
 
         # Define embedding layers
         self.atom_embedding = AtomEmbedding(atom_feature_dim=atom_fea_dim)
-        cutoff_coeff = kwargs.pop("cutoff_coeff", 6)
         self.bond_basis_expansion = BondEncoder(
             atom_graph_cutoff=atom_graph_cutoff,
             bond_graph_cutoff=bond_graph_cutoff,
             num_radial=num_radial,
             cutoff_coeff=cutoff_coeff,
             learnable=learnable_rbf,
         )
@@ -245,26 +248,25 @@
             name=kwargs.pop("readout_norm", None), dim=atom_fea_dim
         )
         self.mlp_first = mlp_first
         if mlp_first:
             self.read_out_type = "sum"
             input_dim = atom_fea_dim
             self.pooling = GraphPooling(average=False)
+        elif read_out in ["attn", "weighted"]:
+            self.read_out_type = "attn"
+            num_heads = kwargs.pop("num_heads", 3)
+            self.pooling = GraphAttentionReadOut(
+                atom_fea_dim, num_head=num_heads, average=True
+            )
+            input_dim = atom_fea_dim * num_heads
         else:
-            if read_out in ["attn", "weighted"]:
-                self.read_out_type = "attn"
-                num_heads = kwargs.pop("num_heads", 3)
-                self.pooling = GraphAttentionReadOut(
-                    atom_fea_dim, num_head=num_heads, average=True
-                )
-                input_dim = atom_fea_dim * num_heads
-            else:
-                self.read_out_type = "ave"
-                input_dim = atom_fea_dim
-                self.pooling = GraphPooling(average=True)
+            self.read_out_type = "ave"
+            input_dim = atom_fea_dim
+            self.pooling = GraphPooling(average=True)
         if kwargs.pop("final_mlp", "MLP") in ["normal", "MLP"]:
             self.mlp = MLP(
                 input_dim=input_dim,
                 hidden_dim=mlp_hidden_dims,
                 output_dim=1,
                 dropout=mlp_dropout,
                 activation=non_linearity,
@@ -514,25 +516,24 @@
             return self.predict_graph(
                 graph,
                 task=task,
                 return_atom_feas=return_atom_feas,
                 return_crystal_feas=return_crystal_feas,
                 batch_size=batch_size,
             )
-        elif type(structure) == list:
+        if type(structure) == list:
             graphs = [self.graph_converter(i) for i in structure]
             return self.predict_graph(
                 graphs,
                 task=task,
                 return_atom_feas=return_atom_feas,
                 return_crystal_feas=return_crystal_feas,
                 batch_size=batch_size,
             )
-        else:
-            raise Exception("input should either be a structure or list of structures!")
+        raise Exception("input should either be a structure or list of structures!")
 
     def predict_graph(
         self,
         graph: CrystalGraph | Sequence[CrystalGraph],
         task: PredTask = "efsm",
         return_atom_feas: bool = False,
         return_crystal_feas: bool = False,
@@ -572,15 +573,15 @@
                     out[key] = pred.item()
                 elif key in ["f", "s", "m", "atom_fea"]:
                     assert len(pred) == 1
                     out[key] = pred[0].cpu().detach().numpy()
                 elif key == "crystal_fea":
                     out[key] = pred.view(-1).cpu().detach().numpy()
             return out
-        elif type(graph) == list:
+        if type(graph) == list:
             self.eval()
             predictions: list[dict[str, Tensor]] = [{} for _ in range(len(graph))]
             n_steps = math.ceil(len(graph) / batch_size)
             for n in range(n_steps):
                 prediction = self.forward(
                     [
                         g.to(model_device)
@@ -604,16 +605,15 @@
                             predictions[n * batch_size + i][key] = (
                                 atom_fea.cpu().detach().numpy()
                             )
                     elif key == "crystal_fea":
                         for i, crystal_fea in enumerate(pred.cpu().detach().numpy()):
                             predictions[n * batch_size + i][key] = crystal_fea
             return predictions
-        else:
-            raise Exception("input should either be a graph or list of graphs!")
+        raise Exception("input should either be a graph or list of graphs!")
 
     @staticmethod
     def split(x: Tensor, n: Tensor) -> Sequence[Tensor]:
         """Split a batched result Tensor into a list of Tensors."""
         print(x, n)
         start = 0
         result = []
@@ -621,41 +621,38 @@
             result.append(x[start : start + i])
             start += i
         assert start == len(x), "Error: source tensor not correctly split!"
         return result
 
     def as_dict(self):
         """Return the CHGNet weights and args in a dictionary."""
-        out = {"state_dict": self.state_dict(), "model_args": self.model_args}
-        return out
+        return {"state_dict": self.state_dict(), "model_args": self.model_args}
 
     @classmethod
     def from_dict(cls, dict, **kwargs):
         """Build a CHGNet from a saved dictionary."""
         chgnet = CHGNet(**dict["model_args"])
         chgnet.load_state_dict(dict["state_dict"], **kwargs)
         return chgnet
 
     @classmethod
     def from_file(cls, path, **kwargs):
         """Build a CHGNet from a saved file."""
         state = torch.load(path, map_location=torch.device("cpu"))
-        chgnet = CHGNet.from_dict(state["model"], **kwargs)
-        return chgnet
+        return CHGNet.from_dict(state["model"], **kwargs)
 
     @classmethod
     def load(cls, model_name="MPtrj-efsm"):
         """Load pretrained CHGNet."""
         current_dir = os.path.dirname(os.path.abspath(__file__))
         if model_name == "MPtrj-efsm":
             return cls.from_file(
                 os.path.join(current_dir, "../pretrained/e30f77s348m32.pth.tar")
             )
-        else:
-            raise Exception("model_name not supported")
+        raise Exception("model_name not supported")
 
 
 @dataclass
 class BatchedGraph:
     """Batched crystal graph for parallel computing.
 
     Attributes:
```

### Comparing `chgnet-0.1.3/chgnet/pretrained/e30f77s348m32.pth.tar` & `chgnet-0.1.4/chgnet/pretrained/e30f77s348m32.pth.tar`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.3/chgnet/trainer/trainer.py` & `chgnet-0.1.4/chgnet/trainer/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,55 +2,56 @@
 
 import datetime
 import inspect
 import os
 import random
 import shutil
 import time
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Literal
 
 import numpy as np
 import torch
 from torch import Tensor, nn
 from torch.optim.lr_scheduler import (
     CosineAnnealingLR,
     CosineAnnealingWarmRestarts,
     ExponentialLR,
     MultiStepLR,
 )
-from torch.utils.data import DataLoader
 
 from chgnet.model.model import CHGNet
 from chgnet.utils import AverageMeter, mae, write_json
 
 if TYPE_CHECKING:
+    from torch.utils.data import DataLoader
+
     from chgnet import TrainTask
 
 
 class Trainer:
     """A trainer to train CHGNet using energy, force, stress and magmom."""
 
     def __init__(
         self,
-        model: nn.Module = None,
+        model: nn.Module | None = None,
         targets: TrainTask = "ef",
         energy_loss_ratio: float = 1,
         force_loss_ratio: float = 1,
         stress_loss_ratio: float = 0.1,
         mag_loss_ratio: float = 0.1,
         optimizer: str = "Adam",
         scheduler: str = "CosLR",
         criterion: str = "MSE",
         epochs: int = 50,
         starting_epoch: int = 0,
         learning_rate: float = 1e-3,
         print_freq: int = 100,
-        torch_seed: int = None,
-        data_seed: int = None,
-        use_device: str = None,
+        torch_seed: int | None = None,
+        data_seed: int | None = None,
+        use_device: str | None = None,
         **kwargs,
     ) -> None:
         """Initialize all hyper-parameters for trainer.
 
         Args:
             model (nn.Module): a CHGNet model
             targets ("ef" | "efs" | "efsm"): The training targets. Default = "ef"
@@ -177,25 +178,25 @@
         # mps is disabled until stable version of torch for mps is released
         # elif torch.backends.mps.is_available():
         #     self.device = "mps"
         else:
             self.device = "cpu"
 
         self.print_freq = print_freq
-        self.training_history = {
-            i: {"train": [], "val": [], "test": []} for i in self.targets
-        }
+        self.training_history: dict[
+            str, dict[Literal["train", "val", "test"], list[float]]
+        ] = {key: {"train": [], "val": [], "test": []} for key in self.targets}
         self.best_model = None
 
     def train(
         self,
         train_loader: DataLoader,
         val_loader: DataLoader,
-        test_loader: DataLoader = None,
-        save_dir: str = None,
+        test_loader: DataLoader | None = None,
+        save_dir: str | None = None,
         save_test_result: bool = False,
     ) -> None:
         """Train the model using torch data_loaders.
 
         Args:
             train_loader (DataLoader): train loader to update CHGNet weights
             val_loader (DataLoader): val loader to test accuracy after each epoch
@@ -270,18 +271,18 @@
         mae_errors = {}
         for i in self.targets:
             mae_errors[i] = AverageMeter()
 
         # switch to train mode
         self.model.train()
 
-        end = time.perf_counter()
+        start = time.perf_counter()  # start timer
         for idx, (graphs, targets) in enumerate(train_loader):
             # measure data loading time
-            data_time.update(time.perf_counter() - end)
+            data_time.update(time.perf_counter() - start)
 
             # get input
             for g in graphs:
                 requires_force = "f" in self.targets
                 g.atom_frac_coord.requires_grad = requires_force
             graphs = [g.to(self.device) for g in graphs]
             targets = {k: self.move_to(v, self.device) for k, v in targets.items()}
@@ -307,34 +308,35 @@
                 self.scheduler.step()
 
             # free memory
             del graphs, targets
             del prediction, combined_loss
 
             # measure elapsed time
-            batch_time.update(time.perf_counter() - end)
+            batch_time.update(time.perf_counter() - start)
+            start = time.perf_counter()
 
             if idx == 0 or (idx + 1) % self.print_freq == 0:
                 message = (
                     f"Epoch: [{current_epoch}][{idx + 1}/{len(train_loader)}]\t"
                     f"Time ({batch_time.avg:.3f})  Data ({data_time.avg:.3f})  "
                     f"Loss {losses.val:.4f} ({losses.avg:.4f})  MAEs:  "
                 )
                 for key in self.targets:
                     message += (
                         f"{key} {mae_errors[key].val:.3f} ({mae_errors[key].avg:.3f})  "
                     )
                 print(message)
-        return {key: round(mae_error.avg, 6) for key, mae_error in mae_errors.items()}
+        return {key: round(err.avg, 6) for key, err in mae_errors.items()}
 
     def _validate(
         self,
         val_loader: DataLoader,
         is_test: bool = False,
-        test_result_save_path: str = None,
+        test_result_save_path: str | None = None,
     ) -> dict:
         """Validation or test step.
 
         Args:
             val_loader (DataLoader): val loader to test accuracy after each epoch
             is_test (bool): whether it's test step
             test_result_save_path (str): path to save test_result
@@ -466,15 +468,15 @@
             "scheduler": self.scheduler.state_dict(),
             "training_history": self.training_history,
             "trainer_args": self.trainer_args,
         }
         torch.save(state, filename)
 
     def save_checkpoint(
-        self, epoch: int, mae_error: dict, save_dir: str = None
+        self, epoch: int, mae_error: dict, save_dir: str | None = None
     ) -> None:
         """Function to save CHGNet trained weights after each epoch.
 
         Args:
             epoch (int): the epoch number
             mae_error (dict): dictionary that stores the mae errors
             save_dir (str): the directory to save trained weights
@@ -538,24 +540,23 @@
         return trainer
 
     @staticmethod
     def move_to(obj, device) -> Tensor | list[Tensor]:
         """Move object to device."""
         if torch.is_tensor(obj):
             return obj.to(device)
-        elif isinstance(obj, list):
+        if isinstance(obj, list):
             out = []
             for tensor in obj:
                 if tensor is not None:
                     out.append(tensor.to(device))
                 else:
                     out.append(None)
             return out
-        else:
-            raise TypeError("Invalid type for move_to")
+        raise TypeError("Invalid type for move_to")
 
 
 class CombinedLoss(nn.Module):
     """A combined loss function of energy, force, stress and magmom."""
 
     def __init__(
         self,
@@ -625,19 +626,21 @@
         Args:
             targets (dict): DFT labels
             prediction (dict): CHGNet prediction
 
         Returns:
             dictionary of all the loss, MAE and MAE_size
         """
-        out: dict[str, Tensor | int] = {"loss": 0}
+        out = {"loss": 0.0}
         # Energy
         if self.energy_loss_ratio != 0 and "e" in targets:
             if self.is_intensive:
-                out["loss"] += self.criterion(targets["e"], prediction["e"])
+                out["loss"] += self.energy_loss_ratio * self.criterion(
+                    targets["e"], prediction["e"]
+                )
                 out["e_MAE"] = mae(targets["e"], prediction["e"])
                 out["e_MAE_size"] = prediction["e"].shape[0]
             else:
                 e_per_atom_target = targets["e"] / prediction["atoms_per_graph"]
                 e_per_atom_pred = prediction["e"] / prediction["atoms_per_graph"]
                 out["loss"] += self.criterion(e_per_atom_target, e_per_atom_pred)
                 out["e_MAE"] = mae(e_per_atom_target, e_per_atom_pred)
```

### Comparing `chgnet-0.1.3/chgnet.egg-info/PKG-INFO` & `chgnet-0.1.4/chgnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: chgnet
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pretrained Universal Neural Network Potential for Charge-informed Atomistic Modeling
 Author-email: Bowen Deng <bowendeng@berkeley.edu>
 License: Modified BSD
 Project-URL: Source, https://github.com/CederGroupHub/chgnet
 Project-URL: Package, https://pypi.org/project/chgnet
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Chemistry
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: crystal-toolkit
 License-File: LICENSE
 
@@ -28,14 +28,15 @@
 
 [![Tests](https://github.com/CederGroupHub/chgnet/actions/workflows/test.yml/badge.svg)](https://github.com/CederGroupHub/chgnet/actions/workflows/test.yml)
 [![Linting](https://github.com/CederGroupHub/chgnet/actions/workflows/lint.yml/badge.svg)](https://github.com/CederGroupHub/chgnet/actions/workflows/lint.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/e3bdcea0382a495d96408e4f84408e85)](https://app.codacy.com/gh/CederGroupHub/chgnet/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 [![arXiv](https://img.shields.io/badge/arXiv-2302.14231-blue)](https://arxiv.org/abs/2302.14231)
 ![GitHub repo size](https://img.shields.io/github/repo-size/CederGroupHub/chgnet)
 [![PyPI](https://img.shields.io/pypi/v/chgnet?logo=pypi&logoColor=white)](https://pypi.org/project/chgnet?logo=pypi&logoColor=white)
+
 </h4>
 
 A pretrained universal neural network potential for
 **charge**-informed atomistic modeling
 ![chgnet](chgnet-logo.png)
 **C**rystal **H**amiltonian **G**raph neural **Net**work is pretrained on the GGA/GGA+U static and relaxation trajectories from Materials Project,
 a comprehensive dataset consisting of 1.5 Million structures from 146k compounds spanning the whole periodic table.
@@ -44,29 +45,28 @@
 in atomistic modeling with near DFT accuracy. The charge inference is realized by regularizing the atom features with
 DFT magnetic moments, which carry rich information about both local ionic environments and charge distribution.
 
 ## Example notebooks
 
 | Notebooks                                                                                                                | Links&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;                                                                                                     | Descriptions                                                                                                                        |
 | ------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
-| [**Using CHGNet**](https://github.com/CederGroupHub/chgnet/blob/main/examples/CHGNet_examples.ipynb)                     | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/CHGNet_examples.ipynb)             | Examples for loading pre-trained CHGNet, predicting energy, force, stress, magmom as well as running structure optimization and MD. |
+| [**CHGNet Basics**](https://github.com/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)                     | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)             | Examples for loading pre-trained CHGNet, predicting energy, force, stress, magmom as well as running structure optimization and MD. |
 | [**Tuning CHGNet**](https://github.com/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                        | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                 | Examples of fine tuning the pretrained CHGNet to your system of interest.                                                           |
 | [**Visualize Relaxation**](https://github.com/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | Crystal Toolkit that visualizes atom positions, energies and forces of a structure during CHGNet relaxation.                        |
 
 [Open in Google Colab]: https://colab.research.google.com/assets/colab-badge.svg
 
 ## Installation
 
 You can install `chgnet` through `pip`:
 
 ```sh
 pip install chgnet
 ```
 
-
 ## Usage
 
 ### Direct Inference (Static Calculation)
 
 Pretrained `CHGNet` can predict the energy (eV/atom), force (eV/A), stress (GPa) and
 magmom ($\mu_B$) of a given structure.
 
@@ -109,15 +109,15 @@
 ```
 
 Visualize the magnetic moments after the MD run
 
 ```python
 from ase.io.trajectory import Trajectory
 from pymatgen.io.ase import AseAtomsAdaptor
-from chgnet.utils.utils import solve_charge_by_mag
+from chgnet.utils import solve_charge_by_mag
 
 traj = Trajectory("md_out.traj")
 mag = traj[-1].get_magnetic_moments()
 
 # get the non-charge-decorated structure
 structure = AseAtomsAdaptor.get_structure(traj[-1])
 print(structure)
```

### Comparing `chgnet-0.1.3/chgnet.egg-info/SOURCES.txt` & `chgnet-0.1.4/chgnet.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
 chgnet/__init__.py
-chgnet/utils.py
 chgnet.egg-info/PKG-INFO
 chgnet.egg-info/SOURCES.txt
 chgnet.egg-info/dependency_links.txt
 chgnet.egg-info/requires.txt
 chgnet.egg-info/top_level.txt
 chgnet/data/__init__.py
 chgnet/data/dataset.py
@@ -21,14 +20,17 @@
 chgnet/model/encoders.py
 chgnet/model/functions.py
 chgnet/model/layers.py
 chgnet/model/model.py
 chgnet/pretrained/e30f77s348m32.pth.tar
 chgnet/trainer/__init__.py
 chgnet/trainer/trainer.py
+chgnet/utils/__init__.py
+chgnet/utils/common_utils.py
+chgnet/utils/vasp_utils.py
 tests/test_converter.py
 tests/test_crystal_graph.py
 tests/test_dataset.py
 tests/test_encoders.py
 tests/test_graph.py
 tests/test_md.py
 tests/test_model.py
```

### Comparing `chgnet-0.1.3/pyproject.toml` & `chgnet-0.1.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chgnet"
-version = "0.1.03"
+version = "0.1.04"
 description = "Pretrained Universal Neural Network Potential for Charge-informed Atomistic Modeling"
 authors = [{ name = "Bowen Deng", email = "bowendeng@berkeley.edu" }]
 requires-python = ">=3.8"
 readme = "README.md"
 license = { text = "Modified BSD" }
 dependencies = [
+    "ase>=3.22.0",
     "numpy>=1.21.6",
-    "torch>=1.11.0",
     "pymatgen>=2022.4.19",
-    "ase>=3.22.0",
+    "torch>=1.11.0",
 ]
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.8",
-    "Topic :: Scientific/Engineering :: Chemistry",
+    "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "Topic :: Scientific/Engineering :: Chemistry",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov"]
 # needed to run interactive example notebooks
-crystal-toolkit = ["crystal-toolkit", "jupyter-dash"]
+crystal-toolkit = ["crystal-toolkit"]
 
 [project.urls]
 Source = "https://github.com/CederGroupHub/chgnet"
 Package = "https://pypi.org/project/chgnet"
 
 [tool.setuptools.packages]
 find = { include = ["chgnet*"], exclude = ["tests", "tests*"] }
@@ -45,37 +45,55 @@
 "chgnet" = ["*.json"]
 "chgnet.pretrained" = ["*.tar"]
 
 [tool.ruff]
 target-version = "py38"
 line-length = 95
 select = [
-    "B",   # flake8-bugbear
-    "D",   # pydocstyle
-    "E",   # pycodestyle
-    "F",   # pyflakes
-    "I",   # isort
-    "PLE", # pylint error
-    "PLW", # pylint warning
-    "PYI", # flakes8-pyi
-    "Q",   # flake8-quotes
-    "SIM", # flake8-simplify
-    "TID", # tidy imports
-    "UP",  # pyupgrade
-    "W",   # pycodestyle
-    "YTT", # flake8-2020
+    "B",    # flake8-bugbear
+    "C4",   # flake8-comprehensions
+    "D",    # pydocstyle
+    "E",    # pycodestyle error
+    "EXE",  # flake8-executable
+    "F",    # pyflakes
+    "FA",   # flake8-future-annotations
+    "FLY",  # flynt
+    "I",    # isort
+    "ICN",  # flake8-import-conventions
+    "ISC",  # flake8-implicit-str-concat
+    "PD",   # pandas-vet
+    "PERF", # perflint
+    "PIE",  # flake8-pie
+    "PL",   # pylint
+    "PT",   # flake8-pytest-style
+    "PYI",  # flakes8-pyi
+    "Q",    # flake8-quotes
+    "RET",  # flake8-return
+    "RSE",  # flake8-raise
+    "RUF",  # Ruff-specific rules
+    "SIM",  # flake8-simplify
+    "SLOT", # flakes8-slot
+    "TCH",  # flake8-type-checking
+    "TID",  # tidy imports
+    "TID",  # flake8-tidy-imports
+    "UP",   # pyupgrade
+    "W",    # pycodestyle warning
+    "YTT",  # flake8-2020
 ]
 ignore = [
     "B019",    # Use of functools.lru_cache on methods can lead to memory leaks
+    "C408",    # unnecessary-collection-call
     "D100",    # Missing docstring in public module
     "D104",    # Missing docstring in public package
     "D205",    # 1 blank line required between summary line and description
+    "PLR",     # pylint refactor
     "PLW2901", # Outer for loop variable overwritten by inner assignment target
-    "SIM105",  # Use contextlib.suppress(FileNotFoundError) instead of try-except-pass
-    "SIM115",  # Use context handler for opening files
+    "PT006",   # pytest-parametrize-names-wrong-type
+    "PT011",   # pytest-raises-too-broad
+    "PT013",   # pytest-incorrect-pytest-import
 ]
 pydocstyle.convention = "google"
 isort.required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["D103"]
 "examples/*" = ["E402"] # E402 Module level import not at top of file
```

### Comparing `chgnet-0.1.3/tests/test_converter.py` & `chgnet-0.1.4/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.3/tests/test_crystal_graph.py` & `chgnet-0.1.4/tests/test_crystal_graph.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.3/tests/test_dataset.py` & `chgnet-0.1.4/tests/test_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,34 +10,33 @@
 
 lattice = Lattice.cubic(4)
 species = ["Na", "Cl"]
 coords = [[0, 0, 0], [0.5, 0.5, 0.5]]
 NaCl = Structure(lattice, species, coords)
 
 
-@pytest.fixture
+@pytest.fixture()
 def structure_data() -> StructureData:
     """Create a graph with 3 nodes and 3 directed edges."""
     structures, energies, forces, stresses, magmoms = [], [], [], [], []
     for _ in range(100):
         struct = NaCl.copy()
         struct.perturb(0.1)
         structures.append(struct)
         energies.append(np.random.random(1))
         forces.append(np.random.random([2, 3]))
         stresses.append(np.random.random([3, 3]))
         magmoms.append(np.random.random([2, 1]))
-    data = StructureData(
+    return StructureData(
         structures=structures,
         energies=energies,
         forces=forces,
         stresses=stresses,
         magmoms=magmoms,
     )
-    return data
 
 
 def test_structure_data(structure_data: StructureData) -> None:
     get_one = structure_data[0]
     assert isinstance(get_one[0], CrystalGraph)
     assert isinstance(get_one[1], dict)
     assert isinstance(get_one[1]["e"], torch.Tensor)
```

### Comparing `chgnet-0.1.3/tests/test_encoders.py` & `chgnet-0.1.4/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.3/tests/test_graph.py` & `chgnet-0.1.4/tests/test_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import pytest
 
 from chgnet.graph.graph import Graph, Node
 
 
-@pytest.fixture
+@pytest.fixture()
 def graph() -> Graph:
     """Create a graph with 3 nodes and 3 directed edges."""
     nodes = [Node(index=idx) for idx in range(3)]
     graph = Graph(nodes)
     graph.add_edge(0, 1, np.array([0, 0, 0]), 1.0)
     graph.add_edge(0, 2, np.array([0, 0, 0]), 2.0)
     graph.add_edge(1, 2, np.array([0, 0, 0]), 3.0)
@@ -46,15 +46,15 @@
     assert len(graph_dict["nodes"]) == 3
     assert len(graph_dict["directed_edges"]) == 0
     assert len(graph_dict["directed_edges_list"]) == 3
     assert len(graph_dict["undirected_edges"]) == 3
     assert len(graph_dict["undirected_edges_list"]) == 3
 
 
-@pytest.fixture
+@pytest.fixture()
 def bigraph() -> Graph:
     """Create a bi-directional graph with 3 nodes and 4 bi-directed edges."""
     nodes = [Node(index=idx) for idx in range(3)]
     bigraph = Graph(nodes)
     bigraph.add_edge(0, 1, np.array([0, 0, 0]), 1.0)
     bigraph.add_edge(0, 2, np.array([0, 0, 0]), 2.0)
     bigraph.add_edge(1, 0, np.array([0, 0, 0]), 1.0)
```

### Comparing `chgnet-0.1.3/tests/test_md.py` & `chgnet-0.1.4/tests/test_md.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
 import os
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 from ase import Atoms
 from ase.md.nptberendsen import Inhomogeneous_NPTBerendsen
 from ase.md.nvtberendsen import NVTBerendsen
 from pymatgen.core import Structure
 from pytest import MonkeyPatch, approx
 
 from chgnet import ROOT
 from chgnet.model import StructOptimizer
 from chgnet.model.dynamics import CHGNetCalculator, EquationOfState, MolecularDynamics
 from chgnet.model.model import CHGNet
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 relaxer = StructOptimizer()
 structure = Structure.from_file(f"{ROOT}/examples/o-LiMnO2_unit.cif")
 chgnet = CHGNet.load()
 
 
 def test_eos():
     eos = EquationOfState()
```

### Comparing `chgnet-0.1.3/tests/test_model.py` & `chgnet-0.1.4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.3/tests/test_relaxation.py` & `chgnet-0.1.4/tests/test_relaxation.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,8 +44,8 @@
 )
 def test_structure_optimizer_passes_kwargs_to_model(use_device) -> None:
     try:
         relaxer = StructOptimizer(use_device=use_device)
         assert relaxer.calculator.device == use_device
     except NotImplementedError as exc:
         # TODO: remove try/except once mps is supported
-        assert str(exc) == "mps is not supported yet"
+        assert str(exc) == "mps is not supported yet"  # noqa: PT017
```

### Comparing `chgnet-0.1.3/tests/test_trainer.py` & `chgnet-0.1.4/tests/test_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     struct = NaCl.copy()
     struct.perturb(0.1)
     structures.append(struct)
     energies.append(np.random.random(1))
     forces.append(np.random.random([2, 3]))
     stresses.append(np.random.random([3, 3]))
     magmoms.append(np.random.random(2))
+
 data = StructureData(
     structures=structures,
     energies=energies,
     forces=forces,
     stresses=stresses,
     magmoms=magmoms,
 )
@@ -44,12 +45,12 @@
     )
     dir_name = "test_tmp_dir"
     test_dir = tmp_path / dir_name
     trainer.train(train_loader, val_loader, save_dir=test_dir)
     assert test_dir.is_dir(), "Training dir was not created"
 
     saved_weight = [f for f in test_dir.iterdir() if f.name.startswith("epoch")]
-    bestE_weight = [f for f in test_dir.iterdir() if f.name.startswith("bestE")]
-    bestF_weight = [f for f in test_dir.iterdir() if f.name.startswith("bestF")]
+    best_e_weight = [f for f in test_dir.iterdir() if f.name.startswith("bestE")]
+    best_f_weight = [f for f in test_dir.iterdir() if f.name.startswith("bestF")]
     assert len(saved_weight) == 1
-    assert len(bestE_weight) == 1
-    assert len(bestF_weight) == 1
+    assert len(best_e_weight) == 1
+    assert len(best_f_weight) == 1
```

