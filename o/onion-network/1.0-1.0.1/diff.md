# Comparing `tmp/onion_network-1.0.tar.gz` & `tmp/onion_network-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onion_network-1.0.tar", last modified: Fri Jun 23 20:38:12 2023, max compression
+gzip compressed data, was "onion_network-1.0.1.tar", last modified: Fri Jun 23 22:23:32 2023, max compression
```

## Comparing `onion_network-1.0.tar` & `onion_network-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:38:12.334034 onion_network-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-23 20:38:02.000000 onion_network-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 20:38:02.000000 onion_network-1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-23 20:38:12.330033 onion_network-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-23 20:38:02.000000 onion_network-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:38:12.330033 onion_network-1.0/onion_network/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-23 20:38:02.000000 onion_network-1.0/onion_network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-23 20:38:02.000000 onion_network-1.0/onion_network/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-23 20:38:02.000000 onion_network-1.0/onion_network/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:38:12.330033 onion_network-1.0/onion_network.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-23 20:38:12.000000 onion_network-1.0/onion_network.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-23 20:38:12.000000 onion_network-1.0/onion_network.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 20:38:12.000000 onion_network-1.0/onion_network.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 20:38:12.000000 onion_network-1.0/onion_network.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 20:38:12.000000 onion_network-1.0/onion_network.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 20:38:02.000000 onion_network-1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 20:38:12.334034 onion_network-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-23 20:38:02.000000 onion_network-1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:38:12.330033 onion_network-1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-23 20:38:02.000000 onion_network-1.0/tests/test_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:23:32.468529 onion_network-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-23 22:23:22.000000 onion_network-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 22:23:22.000000 onion_network-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-23 22:23:32.468529 onion_network-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-06-23 22:23:22.000000 onion_network-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:23:32.468529 onion_network-1.0.1/onion_network/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-23 22:23:22.000000 onion_network-1.0.1/onion_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-23 22:23:22.000000 onion_network-1.0.1/onion_network/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-23 22:23:22.000000 onion_network-1.0.1/onion_network/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:23:32.468529 onion_network-1.0.1/onion_network.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-23 22:23:32.000000 onion_network-1.0.1/onion_network.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-23 22:23:32.000000 onion_network-1.0.1/onion_network.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:23:32.000000 onion_network-1.0.1/onion_network.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 22:23:32.000000 onion_network-1.0.1/onion_network.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 22:23:32.000000 onion_network-1.0.1/onion_network.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 22:23:22.000000 onion_network-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 22:23:32.468529 onion_network-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-23 22:23:22.000000 onion_network-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:23:32.468529 onion_network-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-23 22:23:22.000000 onion_network-1.0.1/tests/test_generation.py
```

### Comparing `onion_network-1.0/LICENSE` & `onion_network-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `onion_network-1.0/README.md` & `onion_network-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,42 +3,57 @@
 <img src="imgs/illustration.png" alt="banner" width="100%">
 
 <p align="center">
 <a href="https://github.com/SimonPop/onion_network/"><img alt="Project Version" src="https://img.shields.io/badge/version-1.0.0-blue"></a>
 <a href="https://www.python.org"><img alt="Python Version 3.8" src="https://img.shields.io/badge/Python-3.8-blue.svg?style=flat&logo=python&logoColor=white"></a>
 <a href="https://github.com/SimonPop/onion_network/LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-blue.svg"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+<a href="https://badge.fury.io/py/onion-network"><img src="https://badge.fury.io/py/onion-network.svg" alt="PyPI version" height="18"></a>
 </p>
 
-Onion-structured networks are special kinds of scale-free networks with a special topologies. They can be decomposed into layers of similar degree nodes.
+Onion-structured networks are special kinds of scale-free networks with special topologies. 
 
-This property gives them a strong resilience to node failure/removal attacks.
+They tend to possess a high degree [assortativity](https://en.wikipedia.org/wiki/Assortativity). It makes it possible to decompose them into layers of same-degree nodes, hence the name.
+
+This property gives them strong resilience to [node deletion](https://en.wikipedia.org/wiki/Node_deletion) attacks.
 
 This library can help you explore these networks, giving access to both a generation and visualization method. 
 
+## Algorithm
+
+A generative algorithm producing synthetic scale-free networks with onion structure is implemented as described in the paper: [Onion structure and network robustness](https://arxiv.org/abs/1108.1841).
+
+> Note: This algorithm can fail under certain circumstances. Therefore a `max_trial` number has been added so that the process can be tried different times until a viable solution is found.
+
+### Visualization
+
+A side module allows plotting the generated graphs, radially separating onion layers.
+
 ## Usage
 
 ### Installation
 
-TODO
+You can install the package using `pip`.
 
-> Note: [(Wu & Holme, 2011)](https://arxiv.org/abs/1108.1841) describe a generation algorithm in their paper. This algorithm is implemented in this  repository. This algorithm can fail under certain circumstances. Therefore a `max_trial` number has been added so that the process can be tried different times.
+```shell
+pip install onion-network
+```
 
 ### Example
 
 ```python
-from onion_network import onion_graph, plot_onion
-
-G = onion_graph(n=100, gamma=2.5, alpha=3., max_trial=1000)
-
+# Example usage of the onion generation and plotting.
+from onion_network import plot_onion, onion_graph
+G = onion_graph(n=100, gamma=2.5, alpha=3, max_trial=100)
 plot_onion(G, cmap="tab20b")
 ```
 
 <img src="imgs/example.png" alt="banner" width="50%" style="display:block;margin-left: auto;margin-right: auto;">
 
+
 ## References
 
 ### Papers
 
 Chan, H., & Akoglu, L. (2016). Optimizing network robustness by edge rewiring : A general framework. Data Mining and Knowledge Discovery, 30(5), 1395‑1425. https://doi.org/10.1007/s10618-015-0447-5
 Chujyo, M., & Hayashi, Y. (2022). Adding links on minimum degree and longest distance strategies for improving network robustness and efficiency. PLOS ONE, 17(10), e0276733. https://doi.org/10.1371/journal.pone.0276733
 Hayashi, Y. (2018). A new design principle of robust onion-like networks self-organized in growth. Network Science, 6(1), 54‑70. https://doi.org/10.1017/nws.2017.25
```

#### html2text {}

```diff
@@ -1,31 +1,39 @@
                        ****** ð§ Onion Network ******
 [banner]
-   [Project_Version] [Python_Version_3.8] [License:_MIT] [Code_style:_black]
-Onion-structured networks are special kinds of scale-free networks with a
-special topologies. They can be decomposed into layers of similar degree nodes.
-This property gives them a strong resilience to node failure/removal attacks.
-This library can help you explore these networks, giving access to both a
-generation and visualization method. ## Usage ### Installation TODO > Note: [
-(Wu & Holme, 2011)](https://arxiv.org/abs/1108.1841) describe a generation
-algorithm in their paper. This algorithm is implemented in this repository.
-This algorithm can fail under certain circumstances. Therefore a `max_trial`
-number has been added so that the process can be tried different times. ###
-Example ```python from onion_network import onion_graph, plot_onion G =
-onion_graph(n=100, gamma=2.5, alpha=3., max_trial=1000) plot_onion(G,
-cmap="tab20b") ``` [banner] ## References ### Papers Chan, H., & Akoglu, L.
-(2016). Optimizing network robustness by edge rewiringâ¯: A general framework.
-Data Mining and Knowledge Discovery, 30(5), 1395â1425. https://doi.org/
-10.1007/s10618-015-0447-5 Chujyo, M., & Hayashi, Y. (2022). Adding links on
-minimum degree and longest distance strategies for improving network robustness
-and efficiency. PLOS ONE, 17(10), e0276733. https://doi.org/10.1371/
-journal.pone.0276733 Hayashi, Y. (2018). A new design principle of robust
-onion-like networks self-organized in growth. Network Science, 6(1), 54â70.
-https://doi.org/10.1017/nws.2017.25 Liu, X., Sun, S., Wang, J., & Xia, C.
-(2019). Onion structure optimizes attack robustness of interdependent networks.
-Physica A: Statistical Mechanics and Its Applications, 535, 122374. https://
-doi.org/10.1016/j.physa.2019.122374 Louzada, V. H. P., Daolio, F., Herrmann, H.
-J., & Tomassini, M. (2013). Smart Rewiring for Network Robustness. Journal of
-Complex Networks, 1(2), 150â159. https://doi.org/10.1093/comnet/cnt010 Wu,
-Z.-X., & Holme, P. (2011, aoÃ»t 9). Onion structure and network robustness.
-ArXiv.Org. https://doi.org/10.1103/PhysRevE.84.026106 ### Blog article [The
-Onion Topology](https://simonpop.github.io/the-onion-topology.html)
+[Project_Version] [Python_Version_3.8] [License:_MIT] [Code_style:_black] [PyPI
+                                   version]
+Onion-structured networks are special kinds of scale-free networks with special
+topologies. They tend to possess a high degree [assortativity](https://
+en.wikipedia.org/wiki/Assortativity). It makes it possible to decompose them
+into layers of same-degree nodes, hence the name. This property gives them
+strong resilience to [node deletion](https://en.wikipedia.org/wiki/
+Node_deletion) attacks. This library can help you explore these networks,
+giving access to both a generation and visualization method. ## Algorithm A
+generative algorithm producing synthetic scale-free networks with onion
+structure is implemented as described in the paper: [Onion structure and
+network robustness](https://arxiv.org/abs/1108.1841). > Note: This algorithm
+can fail under certain circumstances. Therefore a `max_trial` number has been
+added so that the process can be tried different times until a viable solution
+is found. ### Visualization A side module allows plotting the generated graphs,
+radially separating onion layers. ## Usage ### Installation You can install the
+package using `pip`. ```shell pip install onion-network ``` ### Example
+```python # Example usage of the onion generation and plotting. from
+onion_network import plot_onion, onion_graph G = onion_graph(n=100, gamma=2.5,
+alpha=3, max_trial=100) plot_onion(G, cmap="tab20b") ``` [banner] ## References
+### Papers Chan, H., & Akoglu, L. (2016). Optimizing network robustness by edge
+rewiringâ¯: A general framework. Data Mining and Knowledge Discovery, 30(5),
+1395â1425. https://doi.org/10.1007/s10618-015-0447-5 Chujyo, M., & Hayashi,
+Y. (2022). Adding links on minimum degree and longest distance strategies for
+improving network robustness and efficiency. PLOS ONE, 17(10), e0276733. https:
+//doi.org/10.1371/journal.pone.0276733 Hayashi, Y. (2018). A new design
+principle of robust onion-like networks self-organized in growth. Network
+Science, 6(1), 54â70. https://doi.org/10.1017/nws.2017.25 Liu, X., Sun, S.,
+Wang, J., & Xia, C. (2019). Onion structure optimizes attack robustness of
+interdependent networks. Physica A: Statistical Mechanics and Its Applications,
+535, 122374. https://doi.org/10.1016/j.physa.2019.122374 Louzada, V. H. P.,
+Daolio, F., Herrmann, H. J., & Tomassini, M. (2013). Smart Rewiring for Network
+Robustness. Journal of Complex Networks, 1(2), 150â159. https://doi.org/
+10.1093/comnet/cnt010 Wu, Z.-X., & Holme, P. (2011, aoÃ»t 9). Onion structure
+and network robustness. ArXiv.Org. https://doi.org/10.1103/PhysRevE.84.026106
+### Blog article [The Onion Topology](https://simonpop.github.io/the-onion-
+topology.html)
```

### Comparing `onion_network-1.0/onion_network/generation.py` & `onion_network-1.0.1/onion_network/generation.py`

 * *Files identical despite different names*

### Comparing `onion_network-1.0/onion_network/visualization.py` & `onion_network-1.0.1/onion_network/visualization.py`

 * *Files identical despite different names*

### Comparing `onion_network-1.0/setup.py` & `onion_network-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 with open("requirements.txt") as f:
     tests_require = f.readlines()
 install_requires = [t.strip() for t in tests_require]
 
 setup(
     name="onion_network",
-    version="1.0",
+    version="1.0.1",
     description="A module for generating and visualizing onion-structured networks!",
-    long_description="To come",
+    long_description=long_description,
     author="Simon Popelier",
     author_email="simon.popelier@gmail.com",
     packages=["onion_network"],
     install_requires=install_requires,
+    url='https://github.com/SimonPop/onion_network'
 )
```

### Comparing `onion_network-1.0/tests/test_generation.py` & `onion_network-1.0.1/tests/test_generation.py`

 * *Files identical despite different names*

