# Comparing `tmp/pulsars-0.0.5.tar.gz` & `tmp/pulsars-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulsars-0.0.5.tar", max compression
+gzip compressed data, was "pulsars-0.0.6.tar", max compression
```

## Comparing `pulsars-0.0.5.tar` & `pulsars-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2765 2023-06-24 06:48:04.559167 pulsars-0.0.5/README.md
--rw-r--r--   0        0        0     6148 2023-06-12 13:55:15.223860 pulsars-0.0.5/pulsars/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-02 08:36:35.185149 pulsars-0.0.5/pulsars/__init__.py
--rw-r--r--   0        0        0     3265 2023-06-12 06:53:45.765212 pulsars-0.0.5/pulsars/gui/__pycache__/home_page.cpython-310.pyc
--rw-r--r--   0        0        0     1423 2023-06-12 05:37:01.158628 pulsars-0.0.5/pulsars/gui/__pycache__/nabla_geo_page.cpython-310.pyc
--rw-r--r--   0        0        0     2800 2023-06-12 15:19:53.412557 pulsars-0.0.5/pulsars/gui/__pycache__/nabla_home.cpython-310.pyc
--rw-r--r--   0        0        0      423 2023-06-12 12:06:08.881443 pulsars-0.0.5/pulsars/gui/__pycache__/nabla_materials.cpython-310.pyc
--rw-r--r--   0        0        0      415 2023-06-12 12:07:45.921596 pulsars-0.0.5/pulsars/gui/__pycache__/nabla_solver.cpython-310.pyc
--rw-r--r--   0        0        0      373 2023-06-12 15:04:47.224230 pulsars-0.0.5/pulsars/gui/__pycache__/readtoml.cpython-310.pyc
--rw-r--r--   0        0        0      317 2023-06-12 06:15:24.296224 pulsars-0.0.5/pulsars/gui/__pycache__/show_page.cpython-310.pyc
--rw-r--r--   0        0        0      550 2023-06-12 14:00:25.123265 pulsars-0.0.5/pulsars/gui/__pycache__/widgets.cpython-310.pyc
--rw-r--r--   0        0        0     4837 2023-06-12 16:43:56.233765 pulsars-0.0.5/pulsars/gui/app.py
--rw-r--r--   0        0        0   501748 2023-06-11 09:24:27.537826 pulsars-0.0.5/pulsars/gui/assets/pulsars-logo.png
--rw-r--r--   0        0        0   381112 2023-06-09 22:17:58.479336 pulsars-0.0.5/pulsars/gui/assets/pulsars-white.png
--rw-r--r--   0        0        0   441284 2023-06-09 20:49:52.909975 pulsars-0.0.5/pulsars/gui/assets/pulsars.png
--rw-r--r--   0        0        0   224710 2023-06-11 20:33:49.181525 pulsars-0.0.5/pulsars/gui/assets/sps-geo.png
--rw-r--r--   0        0        0        0 2023-06-12 06:24:10.958949 pulsars-0.0.5/pulsars/gui/nabla_geo_page.py
--rw-r--r--   0        0        0     4354 2023-06-12 15:19:53.173762 pulsars-0.0.5/pulsars/gui/nabla_home.py
--rw-r--r--   0        0        0      199 2023-06-12 12:06:08.478321 pulsars-0.0.5/pulsars/gui/nabla_materials.py
--rw-r--r--   0        0        0        0 2023-06-12 11:50:51.690513 pulsars-0.0.5/pulsars/gui/nabla_results.py
--rw-r--r--   0        0        0      192 2023-06-12 12:07:45.465623 pulsars-0.0.5/pulsars/gui/nabla_solver.py
--rw-r--r--   0        0        0       41 2023-06-12 08:24:27.799920 pulsars-0.0.5/pulsars/gui/nabla_style.css
--rw-r--r--   0        0        0       40 2023-06-12 13:45:21.452782 pulsars-0.0.5/pulsars/gui/pulsarsGUI.sh
--rw-r--r--   0        0        0      161 2023-06-12 15:04:46.761133 pulsars-0.0.5/pulsars/gui/readtoml.py
--rw-r--r--   0        0        0      252 2023-06-15 08:46:19.386232 pulsars-0.0.5/pulsars/gui/test.toml
--rw-r--r--   0        0        0      325 2023-06-12 15:19:30.265843 pulsars-0.0.5/pulsars/gui/test1.py
--rw-r--r--   0        0        0      525 2023-06-12 14:00:24.799698 pulsars-0.0.5/pulsars/gui/widgets.py
--rw-r--r--   0        0        0      566 2023-06-24 06:50:46.675673 pulsars-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 pulsars-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2628 2023-06-24 07:19:13.726878 pulsars-0.0.6/README.md
+-rw-r--r--   0        0        0     6148 2023-06-12 13:55:15.223860 pulsars-0.0.6/pulsars/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-02 08:36:35.185149 pulsars-0.0.6/pulsars/__init__.py
+-rw-r--r--   0        0        0     3265 2023-06-12 06:53:45.765212 pulsars-0.0.6/pulsars/gui/__pycache__/home_page.cpython-310.pyc
+-rw-r--r--   0        0        0     1423 2023-06-12 05:37:01.158628 pulsars-0.0.6/pulsars/gui/__pycache__/nabla_geo_page.cpython-310.pyc
+-rw-r--r--   0        0        0     2800 2023-06-12 15:19:53.412557 pulsars-0.0.6/pulsars/gui/__pycache__/nabla_home.cpython-310.pyc
+-rw-r--r--   0        0        0      423 2023-06-12 12:06:08.881443 pulsars-0.0.6/pulsars/gui/__pycache__/nabla_materials.cpython-310.pyc
+-rw-r--r--   0        0        0      415 2023-06-12 12:07:45.921596 pulsars-0.0.6/pulsars/gui/__pycache__/nabla_solver.cpython-310.pyc
+-rw-r--r--   0        0        0      373 2023-06-12 15:04:47.224230 pulsars-0.0.6/pulsars/gui/__pycache__/readtoml.cpython-310.pyc
+-rw-r--r--   0        0        0      317 2023-06-12 06:15:24.296224 pulsars-0.0.6/pulsars/gui/__pycache__/show_page.cpython-310.pyc
+-rw-r--r--   0        0        0      550 2023-06-12 14:00:25.123265 pulsars-0.0.6/pulsars/gui/__pycache__/widgets.cpython-310.pyc
+-rw-r--r--   0        0        0     4837 2023-06-12 16:43:56.233765 pulsars-0.0.6/pulsars/gui/app.py
+-rw-r--r--   0        0        0   501748 2023-06-11 09:24:27.537826 pulsars-0.0.6/pulsars/gui/assets/pulsars-logo.png
+-rw-r--r--   0        0        0   381112 2023-06-09 22:17:58.479336 pulsars-0.0.6/pulsars/gui/assets/pulsars-white.png
+-rw-r--r--   0        0        0   441284 2023-06-09 20:49:52.909975 pulsars-0.0.6/pulsars/gui/assets/pulsars.png
+-rw-r--r--   0        0        0   224710 2023-06-11 20:33:49.181525 pulsars-0.0.6/pulsars/gui/assets/sps-geo.png
+-rw-r--r--   0        0        0        0 2023-06-12 06:24:10.958949 pulsars-0.0.6/pulsars/gui/nabla_geo_page.py
+-rw-r--r--   0        0        0     4354 2023-06-12 15:19:53.173762 pulsars-0.0.6/pulsars/gui/nabla_home.py
+-rw-r--r--   0        0        0      199 2023-06-12 12:06:08.478321 pulsars-0.0.6/pulsars/gui/nabla_materials.py
+-rw-r--r--   0        0        0        0 2023-06-12 11:50:51.690513 pulsars-0.0.6/pulsars/gui/nabla_results.py
+-rw-r--r--   0        0        0      192 2023-06-12 12:07:45.465623 pulsars-0.0.6/pulsars/gui/nabla_solver.py
+-rw-r--r--   0        0        0       41 2023-06-12 08:24:27.799920 pulsars-0.0.6/pulsars/gui/nabla_style.css
+-rw-r--r--   0        0        0       40 2023-06-12 13:45:21.452782 pulsars-0.0.6/pulsars/gui/pulsarsGUI.sh
+-rw-r--r--   0        0        0      161 2023-06-12 15:04:46.761133 pulsars-0.0.6/pulsars/gui/readtoml.py
+-rw-r--r--   0        0        0      252 2023-06-15 08:46:19.386232 pulsars-0.0.6/pulsars/gui/test.toml
+-rw-r--r--   0        0        0      325 2023-06-12 15:19:30.265843 pulsars-0.0.6/pulsars/gui/test1.py
+-rw-r--r--   0        0        0      525 2023-06-12 14:00:24.799698 pulsars-0.0.6/pulsars/gui/widgets.py
+-rw-r--r--   0        0        0      566 2023-06-24 06:59:20.360590 pulsars-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3443 1970-01-01 00:00:00.000000 pulsars-0.0.6/PKG-INFO
```

### Comparing `pulsars-0.0.5/README.md` & `pulsars-0.0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# <img src="./assets/logo-pulsars-bg.png" alt="Image Title" width="800" height="auto">
+
+# <img src="https://raw.githubusercontent.com/altar31/altar31/fd3133b864f207c7633112e75399e910b49959c8/public/logo-pulsars-bg.png" alt="Image Title" width="800" height="auto">
 
 ## ☕️ About
-**Pulsars** (pronounced "Pulsar") is a **building** and **Command Line Interface (CLI)** system for helping researchers and engineers to **practically** use [Machine Learning (ML)](https://en.wikipedia.org/wiki/Machine_learning), [Deep Learning (DL)](https://en.wikipedia.org/wiki/Deep_learning) algorithms.
+**Pulsars** (pronounced "Pulsar") is a system for helping researchers and engineers to **practically** use [Machine Learning (ML)](https://en.wikipedia.org/wiki/Machine_learning), [Deep Learning (DL)](https://en.wikipedia.org/wiki/Deep_learning) algorithms.
 
 
 **Pulsars** is based on **configuration files** and **CLI**. In other words, it takes an **input configuration file** in the [TOML](https://toml.io/en/) format with a **domain specific semantics** and generate **automatically** the associated python code.
 In that way, the user only write (or use template) **configurations files** and run the whole system through the **CLI**.
 
-Thus, the user can focus on the problem without to manage the **cumberstone stuff** and **complex python codes**, generally involved for building ML/DL models.
+Thus, the user can focus on the problem without to manage the **cumberstone stuff** and **complex python codes**, generally involved for building and training ML/DL models.
 
 
 ## ⁉️ Why
 Because at first, researchers and engineers are not necessary **Python programmers** or **ML specialists**. 
 In addition, even for **specialists**, we want to bring a different way of building such complex systems with **productivity** in minds.
 
 ## Built on the Python ecosystem
 
-We do not want to **reinvent the wheel**, that's why **Pulsars** is built upon **Python ML/DL/FEM ecosystem**. 
+We do not want to **reinvent the wheel**, that's why **Pulsars** is built upon **Python ML/DL ecosystem**. 
 
 - 🔁 Machine Learning Lifecycle ([mlflow](https://mlflow.org/))
 - 🤖 Machine Learning Algorithms ([XGBoost](https://xgboost.readthedocs.io/en/stable/)...)
 - 🕸️ Deep Learning Algorithms ([Keras](https://keras.io/), [Tensorflow](https://www.tensorflow.org/))
 - 🛠️ Hyperparameters Tuning ([Ray Tune](https://docs.ray.io/en/latest/tune/index.html))
 - 📈 Results visualization ([Matplotlib](https://matplotlib.org/), [Seaborn](https://seaborn.pydata.org/index.html))
 
@@ -40,24 +41,17 @@
 pip install pulsars
 ```
 
 ## For developement
 
 ### 🔗 Dependencies
 
-- Install [Conda](https://www.anaconda.com/) package management tool
-
-```bash
-git clone https://github.com/altar31/pulsars
-cd pulsars
-conda env create -f environment.yaml 
-conda activate pulsars
-```
+To do ...
 
 ## ⚠️ Under construction
 This project is at the **early developement stage** and is truly **experimental**.
 This mean **most** of the features are **missing** and the documentation is still **lacking**.
 The project **github** repository will be available soon ! Stay tuned !
-After the public release of the github repository, contributions of any kinds (code, documentation, logo, community ...) will be really welcome !😁
+After the public release of the github repository, contributions of any kinds (code, documentation, website, community ...) will be really welcome !😁
```

### Comparing `pulsars-0.0.5/pulsars/.DS_Store` & `pulsars-0.0.6/pulsars/.DS_Store`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.5/pulsars/gui/__pycache__/home_page.cpython-310.pyc` & `pulsars-0.0.6/pulsars/gui/__pycache__/home_page.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.5/pulsars/gui/__pycache__/nabla_geo_page.cpython-310.pyc` & `pulsars-0.0.6/pulsars/gui/__pycache__/nabla_geo_page.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.5/pulsars/gui/__pycache__/nabla_home.cpython-310.pyc` & `pulsars-0.0.6/pulsars/gui/__pycache__/nabla_home.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.5/pulsars/gui/__pycache__/widgets.cpython-310.pyc` & `pulsars-0.0.6/pulsars/gui/__pycache__/widgets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.5/pulsars/gui/app.py` & `pulsars-0.0.6/pulsars/gui/app.py`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.5/pulsars/gui/assets/pulsars-logo.png` & `pulsars-0.0.6/pulsars/gui/assets/pulsars-logo.png`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.5/pulsars/gui/assets/pulsars-white.png` & `pulsars-0.0.6/pulsars/gui/assets/pulsars-white.png`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.5/pulsars/gui/assets/pulsars.png` & `pulsars-0.0.6/pulsars/gui/assets/pulsars.png`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.5/pulsars/gui/assets/sps-geo.png` & `pulsars-0.0.6/pulsars/gui/assets/sps-geo.png`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.5/pulsars/gui/nabla_home.py` & `pulsars-0.0.6/pulsars/gui/nabla_home.py`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.5/pulsars/gui/widgets.py` & `pulsars-0.0.6/pulsars/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `pulsars-0.0.5/pyproject.toml` & `pulsars-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pulsars"
-version = "0.0.5"
+version = "0.0.6"
 description = "A Practical Machine Learning System for Applied Research"
 authors = ["altar31 <damien.sicard31@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pulsars-0.0.5/PKG-INFO` & `pulsars-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsars
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Practical Machine Learning System for Applied Research
 License: MIT
 Author: altar31
 Author-email: damien.sicard31@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,33 +17,34 @@
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: xgboost (>=1.7.6,<2.0.0)
 Description-Content-Type: text/markdown
 
-# <img src="./assets/logo-pulsars-bg.png" alt="Image Title" width="800" height="auto">
+
+# <img src="https://raw.githubusercontent.com/altar31/altar31/fd3133b864f207c7633112e75399e910b49959c8/public/logo-pulsars-bg.png" alt="Image Title" width="800" height="auto">
 
 ## ☕️ About
-**Pulsars** (pronounced "Pulsar") is a **building** and **Command Line Interface (CLI)** system for helping researchers and engineers to **practically** use [Machine Learning (ML)](https://en.wikipedia.org/wiki/Machine_learning), [Deep Learning (DL)](https://en.wikipedia.org/wiki/Deep_learning) algorithms.
+**Pulsars** (pronounced "Pulsar") is a system for helping researchers and engineers to **practically** use [Machine Learning (ML)](https://en.wikipedia.org/wiki/Machine_learning), [Deep Learning (DL)](https://en.wikipedia.org/wiki/Deep_learning) algorithms.
 
 
 **Pulsars** is based on **configuration files** and **CLI**. In other words, it takes an **input configuration file** in the [TOML](https://toml.io/en/) format with a **domain specific semantics** and generate **automatically** the associated python code.
 In that way, the user only write (or use template) **configurations files** and run the whole system through the **CLI**.
 
-Thus, the user can focus on the problem without to manage the **cumberstone stuff** and **complex python codes**, generally involved for building ML/DL models.
+Thus, the user can focus on the problem without to manage the **cumberstone stuff** and **complex python codes**, generally involved for building and training ML/DL models.
 
 
 ## ⁉️ Why
 Because at first, researchers and engineers are not necessary **Python programmers** or **ML specialists**. 
 In addition, even for **specialists**, we want to bring a different way of building such complex systems with **productivity** in minds.
 
 ## Built on the Python ecosystem
 
-We do not want to **reinvent the wheel**, that's why **Pulsars** is built upon **Python ML/DL/FEM ecosystem**. 
+We do not want to **reinvent the wheel**, that's why **Pulsars** is built upon **Python ML/DL ecosystem**. 
 
 - 🔁 Machine Learning Lifecycle ([mlflow](https://mlflow.org/))
 - 🤖 Machine Learning Algorithms ([XGBoost](https://xgboost.readthedocs.io/en/stable/)...)
 - 🕸️ Deep Learning Algorithms ([Keras](https://keras.io/), [Tensorflow](https://www.tensorflow.org/))
 - 🛠️ Hyperparameters Tuning ([Ray Tune](https://docs.ray.io/en/latest/tune/index.html))
 - 📈 Results visualization ([Matplotlib](https://matplotlib.org/), [Seaborn](https://seaborn.pydata.org/index.html))
 
@@ -63,25 +64,18 @@
 pip install pulsars
 ```
 
 ## For developement
 
 ### 🔗 Dependencies
 
-- Install [Conda](https://www.anaconda.com/) package management tool
-
-```bash
-git clone https://github.com/altar31/pulsars
-cd pulsars
-conda env create -f environment.yaml 
-conda activate pulsars
-```
+To do ...
 
 ## ⚠️ Under construction
 This project is at the **early developement stage** and is truly **experimental**.
 This mean **most** of the features are **missing** and the documentation is still **lacking**.
 The project **github** repository will be available soon ! Stay tuned !
-After the public release of the github repository, contributions of any kinds (code, documentation, logo, community ...) will be really welcome !😁
+After the public release of the github repository, contributions of any kinds (code, documentation, website, community ...) will be really welcome !😁
```

