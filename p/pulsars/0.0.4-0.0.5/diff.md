# Comparing `tmp/pulsars-0.0.4.tar.gz` & `tmp/pulsars-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulsars-0.0.4.tar", max compression
+gzip compressed data, was "pulsars-0.0.5.tar", max compression
```

## Comparing `pulsars-0.0.4.tar` & `pulsars-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     3462 2023-06-23 16:38:51.814347 pulsars-0.0.4/README.md
--rw-r--r--   0        0        0     6148 2023-06-12 13:55:15.223860 pulsars-0.0.4/pulsars/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-02 08:36:35.185149 pulsars-0.0.4/pulsars/__init__.py
--rw-r--r--   0        0        0     3265 2023-06-12 06:53:45.765212 pulsars-0.0.4/pulsars/gui/__pycache__/home_page.cpython-310.pyc
--rw-r--r--   0        0        0     1423 2023-06-12 05:37:01.158628 pulsars-0.0.4/pulsars/gui/__pycache__/nabla_geo_page.cpython-310.pyc
--rw-r--r--   0        0        0     2800 2023-06-12 15:19:53.412557 pulsars-0.0.4/pulsars/gui/__pycache__/nabla_home.cpython-310.pyc
--rw-r--r--   0        0        0      423 2023-06-12 12:06:08.881443 pulsars-0.0.4/pulsars/gui/__pycache__/nabla_materials.cpython-310.pyc
--rw-r--r--   0        0        0      415 2023-06-12 12:07:45.921596 pulsars-0.0.4/pulsars/gui/__pycache__/nabla_solver.cpython-310.pyc
--rw-r--r--   0        0        0      373 2023-06-12 15:04:47.224230 pulsars-0.0.4/pulsars/gui/__pycache__/readtoml.cpython-310.pyc
--rw-r--r--   0        0        0      317 2023-06-12 06:15:24.296224 pulsars-0.0.4/pulsars/gui/__pycache__/show_page.cpython-310.pyc
--rw-r--r--   0        0        0      550 2023-06-12 14:00:25.123265 pulsars-0.0.4/pulsars/gui/__pycache__/widgets.cpython-310.pyc
--rw-r--r--   0        0        0     4837 2023-06-12 16:43:56.233765 pulsars-0.0.4/pulsars/gui/app.py
--rw-r--r--   0        0        0   501748 2023-06-11 09:24:27.537826 pulsars-0.0.4/pulsars/gui/assets/pulsars-logo.png
--rw-r--r--   0        0        0   381112 2023-06-09 22:17:58.479336 pulsars-0.0.4/pulsars/gui/assets/pulsars-white.png
--rw-r--r--   0        0        0   441284 2023-06-09 20:49:52.909975 pulsars-0.0.4/pulsars/gui/assets/pulsars.png
--rw-r--r--   0        0        0   224710 2023-06-11 20:33:49.181525 pulsars-0.0.4/pulsars/gui/assets/sps-geo.png
--rw-r--r--   0        0        0        0 2023-06-12 06:24:10.958949 pulsars-0.0.4/pulsars/gui/nabla_geo_page.py
--rw-r--r--   0        0        0     4354 2023-06-12 15:19:53.173762 pulsars-0.0.4/pulsars/gui/nabla_home.py
--rw-r--r--   0        0        0      199 2023-06-12 12:06:08.478321 pulsars-0.0.4/pulsars/gui/nabla_materials.py
--rw-r--r--   0        0        0        0 2023-06-12 11:50:51.690513 pulsars-0.0.4/pulsars/gui/nabla_results.py
--rw-r--r--   0        0        0      192 2023-06-12 12:07:45.465623 pulsars-0.0.4/pulsars/gui/nabla_solver.py
--rw-r--r--   0        0        0       41 2023-06-12 08:24:27.799920 pulsars-0.0.4/pulsars/gui/nabla_style.css
--rw-r--r--   0        0        0       40 2023-06-12 13:45:21.452782 pulsars-0.0.4/pulsars/gui/pulsarsGUI.sh
--rw-r--r--   0        0        0      161 2023-06-12 15:04:46.761133 pulsars-0.0.4/pulsars/gui/readtoml.py
--rw-r--r--   0        0        0      252 2023-06-15 08:46:19.386232 pulsars-0.0.4/pulsars/gui/test.toml
--rw-r--r--   0        0        0      325 2023-06-12 15:19:30.265843 pulsars-0.0.4/pulsars/gui/test1.py
--rw-r--r--   0        0        0      525 2023-06-12 14:00:24.799698 pulsars-0.0.4/pulsars/gui/widgets.py
--rw-r--r--   0        0        0      403 2023-06-22 19:47:42.932339 pulsars-0.0.4/pulsars/templates/sps/sps_v0.py
--rw-r--r--   0        0        0      400 2023-06-23 16:38:35.889025 pulsars-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3921 1970-01-01 00:00:00.000000 pulsars-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2765 2023-06-24 06:48:04.559167 pulsars-0.0.5/README.md
+-rw-r--r--   0        0        0     6148 2023-06-12 13:55:15.223860 pulsars-0.0.5/pulsars/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-02 08:36:35.185149 pulsars-0.0.5/pulsars/__init__.py
+-rw-r--r--   0        0        0     3265 2023-06-12 06:53:45.765212 pulsars-0.0.5/pulsars/gui/__pycache__/home_page.cpython-310.pyc
+-rw-r--r--   0        0        0     1423 2023-06-12 05:37:01.158628 pulsars-0.0.5/pulsars/gui/__pycache__/nabla_geo_page.cpython-310.pyc
+-rw-r--r--   0        0        0     2800 2023-06-12 15:19:53.412557 pulsars-0.0.5/pulsars/gui/__pycache__/nabla_home.cpython-310.pyc
+-rw-r--r--   0        0        0      423 2023-06-12 12:06:08.881443 pulsars-0.0.5/pulsars/gui/__pycache__/nabla_materials.cpython-310.pyc
+-rw-r--r--   0        0        0      415 2023-06-12 12:07:45.921596 pulsars-0.0.5/pulsars/gui/__pycache__/nabla_solver.cpython-310.pyc
+-rw-r--r--   0        0        0      373 2023-06-12 15:04:47.224230 pulsars-0.0.5/pulsars/gui/__pycache__/readtoml.cpython-310.pyc
+-rw-r--r--   0        0        0      317 2023-06-12 06:15:24.296224 pulsars-0.0.5/pulsars/gui/__pycache__/show_page.cpython-310.pyc
+-rw-r--r--   0        0        0      550 2023-06-12 14:00:25.123265 pulsars-0.0.5/pulsars/gui/__pycache__/widgets.cpython-310.pyc
+-rw-r--r--   0        0        0     4837 2023-06-12 16:43:56.233765 pulsars-0.0.5/pulsars/gui/app.py
+-rw-r--r--   0        0        0   501748 2023-06-11 09:24:27.537826 pulsars-0.0.5/pulsars/gui/assets/pulsars-logo.png
+-rw-r--r--   0        0        0   381112 2023-06-09 22:17:58.479336 pulsars-0.0.5/pulsars/gui/assets/pulsars-white.png
+-rw-r--r--   0        0        0   441284 2023-06-09 20:49:52.909975 pulsars-0.0.5/pulsars/gui/assets/pulsars.png
+-rw-r--r--   0        0        0   224710 2023-06-11 20:33:49.181525 pulsars-0.0.5/pulsars/gui/assets/sps-geo.png
+-rw-r--r--   0        0        0        0 2023-06-12 06:24:10.958949 pulsars-0.0.5/pulsars/gui/nabla_geo_page.py
+-rw-r--r--   0        0        0     4354 2023-06-12 15:19:53.173762 pulsars-0.0.5/pulsars/gui/nabla_home.py
+-rw-r--r--   0        0        0      199 2023-06-12 12:06:08.478321 pulsars-0.0.5/pulsars/gui/nabla_materials.py
+-rw-r--r--   0        0        0        0 2023-06-12 11:50:51.690513 pulsars-0.0.5/pulsars/gui/nabla_results.py
+-rw-r--r--   0        0        0      192 2023-06-12 12:07:45.465623 pulsars-0.0.5/pulsars/gui/nabla_solver.py
+-rw-r--r--   0        0        0       41 2023-06-12 08:24:27.799920 pulsars-0.0.5/pulsars/gui/nabla_style.css
+-rw-r--r--   0        0        0       40 2023-06-12 13:45:21.452782 pulsars-0.0.5/pulsars/gui/pulsarsGUI.sh
+-rw-r--r--   0        0        0      161 2023-06-12 15:04:46.761133 pulsars-0.0.5/pulsars/gui/readtoml.py
+-rw-r--r--   0        0        0      252 2023-06-15 08:46:19.386232 pulsars-0.0.5/pulsars/gui/test.toml
+-rw-r--r--   0        0        0      325 2023-06-12 15:19:30.265843 pulsars-0.0.5/pulsars/gui/test1.py
+-rw-r--r--   0        0        0      525 2023-06-12 14:00:24.799698 pulsars-0.0.5/pulsars/gui/widgets.py
+-rw-r--r--   0        0        0      566 2023-06-24 06:50:46.675673 pulsars-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 pulsars-0.0.5/PKG-INFO
```

### Comparing `pulsars-0.0.4/README.md` & `pulsars-0.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,33 @@
-# <img src="./Assets/full-logo-pulsars.png" alt="Image Title" width="800" height="auto">
+# <img src="./assets/logo-pulsars-bg.png" alt="Image Title" width="800" height="auto">
 
 ## ☕️ About
-**Pulsars** (pronounced "Pulsar") is a **building** and **Command Line Interface (CLI)** system to help researchers, engineers to **practically** use [Machine Learning (ML)](https://en.wikipedia.org/wiki/Machine_learning), [Deep Learning](https://en.wikipedia.org/wiki/Deep_learning) algorithms and/or solve [Partial Differential Equations](https://en.wikipedia.org/wiki/Partial_differential_equation) using the [Finite Element Method (FEM)](https://en.wikipedia.org/wiki/Finite_element_method).
+**Pulsars** (pronounced "Pulsar") is a **building** and **Command Line Interface (CLI)** system for helping researchers and engineers to **practically** use [Machine Learning (ML)](https://en.wikipedia.org/wiki/Machine_learning), [Deep Learning (DL)](https://en.wikipedia.org/wiki/Deep_learning) algorithms.
 
 
-**Pulsars** is based on **configuration files** and **CLI**. In other words, it takes an **input configuration file** in the [YAML](https://yaml.org/) format with a **domain specific semantics** and generate **automatically** the associated python code.
+**Pulsars** is based on **configuration files** and **CLI**. In other words, it takes an **input configuration file** in the [TOML](https://toml.io/en/) format with a **domain specific semantics** and generate **automatically** the associated python code.
 In that way, the user only write (or use template) **configurations files** and run the whole system through the **CLI**.
 
-Thus, the user can focus on the problem without to manage the **cumberstone stuff** and **complex python codes**, generally involved for building ML/DL models or numerical simulations.
+Thus, the user can focus on the problem without to manage the **cumberstone stuff** and **complex python codes**, generally involved for building ML/DL models.
 
 
 ## ⁉️ Why
-Because at first, researchers and engineers are not necessary **Python programmers** or **ML/DL/FEM specialists**. 
+Because at first, researchers and engineers are not necessary **Python programmers** or **ML specialists**. 
 In addition, even for **specialists**, we want to bring a different way of building such complex systems with **productivity** in minds.
 
 ## Built on the Python ecosystem
 
 We do not want to **reinvent the wheel**, that's why **Pulsars** is built upon **Python ML/DL/FEM ecosystem**. 
 
-The Pulsars library is composed of two main components which could be used together or independently:
-
-### PulseML: The Machine Learning Side
 - 🔁 Machine Learning Lifecycle ([mlflow](https://mlflow.org/))
 - 🤖 Machine Learning Algorithms ([XGBoost](https://xgboost.readthedocs.io/en/stable/)...)
 - 🕸️ Deep Learning Algorithms ([Keras](https://keras.io/), [Tensorflow](https://www.tensorflow.org/))
 - 🛠️ Hyperparameters Tuning ([Ray Tune](https://docs.ray.io/en/latest/tune/index.html))
 - 📈 Results visualization ([Matplotlib](https://matplotlib.org/), [Seaborn](https://seaborn.pydata.org/index.html))
 
-### PulseSIM: The Numerical Simulation Side
-- 🕸️ Mesh generation ([Gmsh](https://gmsh.info/),[Meshio](https://github.com/nschloe/meshio) ) 
-- ⚙️ Efficient FEM solver ([FEniCSx](https://fenicsproject.org/))
-- 📈 Results visualization ([Matplotlib](https://matplotlib.org/), [Seaborn](https://seaborn.pydata.org/index.html))
-
 ### The Command Line Interface (CLI)
 Pulsars provide an expressive CLI to manage and run the whole system 
 
 - [Click](https://panel.holoviz.org/index.html)
 
 ## 📚 Documentation
```

### Comparing `pulsars-0.0.4/pulsars/.DS_Store` & `pulsars-0.0.5/pulsars/.DS_Store`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.4/pulsars/gui/__pycache__/home_page.cpython-310.pyc` & `pulsars-0.0.5/pulsars/gui/__pycache__/home_page.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.4/pulsars/gui/__pycache__/nabla_geo_page.cpython-310.pyc` & `pulsars-0.0.5/pulsars/gui/__pycache__/nabla_geo_page.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.4/pulsars/gui/__pycache__/nabla_home.cpython-310.pyc` & `pulsars-0.0.5/pulsars/gui/__pycache__/nabla_home.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.4/pulsars/gui/__pycache__/widgets.cpython-310.pyc` & `pulsars-0.0.5/pulsars/gui/__pycache__/widgets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.4/pulsars/gui/app.py` & `pulsars-0.0.5/pulsars/gui/app.py`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.4/pulsars/gui/assets/pulsars-logo.png` & `pulsars-0.0.5/pulsars/gui/assets/pulsars-logo.png`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.4/pulsars/gui/assets/pulsars-white.png` & `pulsars-0.0.5/pulsars/gui/assets/pulsars-white.png`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.4/pulsars/gui/assets/pulsars.png` & `pulsars-0.0.5/pulsars/gui/assets/pulsars.png`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.4/pulsars/gui/assets/sps-geo.png` & `pulsars-0.0.5/pulsars/gui/assets/sps-geo.png`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.4/pulsars/gui/nabla_home.py` & `pulsars-0.0.5/pulsars/gui/nabla_home.py`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.4/pulsars/gui/widgets.py` & `pulsars-0.0.5/pulsars/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.4/PKG-INFO` & `pulsars-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 Metadata-Version: 2.1
 Name: pulsars
-Version: 0.0.4
-Summary: A Practical Machine Learning & Simulation Building System
+Version: 0.0.5
+Summary: A Practical Machine Learning System for Applied Research
 License: MIT
 Author: altar31
 Author-email: damien.sicard31@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: keras (>=2.12.0,<3.0.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: mlflow (>=2.4.1,<3.0.0)
+Requires-Dist: numpy (>=1.25.0,<2.0.0)
+Requires-Dist: pandas (>=2.0.2,<3.0.0)
+Requires-Dist: seaborn (>=0.12.2,<0.13.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: xgboost (>=1.7.6,<2.0.0)
 Description-Content-Type: text/markdown
 
-# <img src="./Assets/full-logo-pulsars.png" alt="Image Title" width="800" height="auto">
+# <img src="./assets/logo-pulsars-bg.png" alt="Image Title" width="800" height="auto">
 
 ## ☕️ About
-**Pulsars** (pronounced "Pulsar") is a **building** and **Command Line Interface (CLI)** system to help researchers, engineers to **practically** use [Machine Learning (ML)](https://en.wikipedia.org/wiki/Machine_learning), [Deep Learning](https://en.wikipedia.org/wiki/Deep_learning) algorithms and/or solve [Partial Differential Equations](https://en.wikipedia.org/wiki/Partial_differential_equation) using the [Finite Element Method (FEM)](https://en.wikipedia.org/wiki/Finite_element_method).
+**Pulsars** (pronounced "Pulsar") is a **building** and **Command Line Interface (CLI)** system for helping researchers and engineers to **practically** use [Machine Learning (ML)](https://en.wikipedia.org/wiki/Machine_learning), [Deep Learning (DL)](https://en.wikipedia.org/wiki/Deep_learning) algorithms.
 
 
-**Pulsars** is based on **configuration files** and **CLI**. In other words, it takes an **input configuration file** in the [YAML](https://yaml.org/) format with a **domain specific semantics** and generate **automatically** the associated python code.
+**Pulsars** is based on **configuration files** and **CLI**. In other words, it takes an **input configuration file** in the [TOML](https://toml.io/en/) format with a **domain specific semantics** and generate **automatically** the associated python code.
 In that way, the user only write (or use template) **configurations files** and run the whole system through the **CLI**.
 
-Thus, the user can focus on the problem without to manage the **cumberstone stuff** and **complex python codes**, generally involved for building ML/DL models or numerical simulations.
+Thus, the user can focus on the problem without to manage the **cumberstone stuff** and **complex python codes**, generally involved for building ML/DL models.
 
 
 ## ⁉️ Why
-Because at first, researchers and engineers are not necessary **Python programmers** or **ML/DL/FEM specialists**. 
+Because at first, researchers and engineers are not necessary **Python programmers** or **ML specialists**. 
 In addition, even for **specialists**, we want to bring a different way of building such complex systems with **productivity** in minds.
 
 ## Built on the Python ecosystem
 
 We do not want to **reinvent the wheel**, that's why **Pulsars** is built upon **Python ML/DL/FEM ecosystem**. 
 
-The Pulsars library is composed of two main components which could be used together or independently:
-
-### PulseML: The Machine Learning Side
 - 🔁 Machine Learning Lifecycle ([mlflow](https://mlflow.org/))
 - 🤖 Machine Learning Algorithms ([XGBoost](https://xgboost.readthedocs.io/en/stable/)...)
 - 🕸️ Deep Learning Algorithms ([Keras](https://keras.io/), [Tensorflow](https://www.tensorflow.org/))
 - 🛠️ Hyperparameters Tuning ([Ray Tune](https://docs.ray.io/en/latest/tune/index.html))
 - 📈 Results visualization ([Matplotlib](https://matplotlib.org/), [Seaborn](https://seaborn.pydata.org/index.html))
 
-### PulseSIM: The Numerical Simulation Side
-- 🕸️ Mesh generation ([Gmsh](https://gmsh.info/),[Meshio](https://github.com/nschloe/meshio) ) 
-- ⚙️ Efficient FEM solver ([FEniCSx](https://fenicsproject.org/))
-- 📈 Results visualization ([Matplotlib](https://matplotlib.org/), [Seaborn](https://seaborn.pydata.org/index.html))
-
 ### The Command Line Interface (CLI)
 Pulsars provide an expressive CLI to manage and run the whole system 
 
 - [Click](https://panel.holoviz.org/index.html)
 
 ## 📚 Documentation
```

