# Comparing `tmp/jaxip-0.6.0.tar.gz` & `tmp/jaxip-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxip-0.6.0.tar", last modified: Sun Jun 18 10:02:54 2023, max compression
+gzip compressed data, was "jaxip-0.6.1.tar", last modified: Sat Jun 24 19:26:59 2023, max compression
```

## Comparing `jaxip-0.6.0.tar` & `jaxip-0.6.1.tar`

### file list

```diff
@@ -1,147 +1,151 @@
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.381492 jaxip-0.6.0/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.6.0/AUTHORS.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.6.0/CONTRIBUTING.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      650 2023-06-18 10:02:01.000000 jaxip-0.6.0/HISTORY.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.6.0/LICENSE
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.6.0/MANIFEST.in
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5332 2023-06-18 10:02:54.381492 jaxip-0.6.0/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4745 2023-05-17 19:30:18.000000 jaxip-0.6.0/README.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.357491 jaxip-0.6.0/docs/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.6.0/docs/Makefile
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.349491 jaxip-0.6.0/docs/_build/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.349491 jaxip-0.6.0/docs/_build/doctrees/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.357491 jaxip-0.6.0/docs/_build/doctrees/nbsphinx/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-06-18 09:34:19.000000 jaxip-0.6.0/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-06-18 09:34:19.000000 jaxip-0.6.0/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-06-18 09:34:19.000000 jaxip-0.6.0/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.349491 jaxip-0.6.0/docs/_build/html/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.357491 jaxip-0.6.0/docs/_build/html/_images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-06-18 09:20:05.000000 jaxip-0.6.0/docs/_build/html/_images/notebooks_tutorials_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-06-18 09:20:05.000000 jaxip-0.6.0/docs/_build/html/_images/notebooks_tutorials_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-06-18 09:20:05.000000 jaxip-0.6.0/docs/_build/html/_images/notebooks_tutorials_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.357491 jaxip-0.6.0/docs/_build/html/_static/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.6.0/docs/_build/html/_static/file.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.6.0/docs/_build/html/_static/minus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.6.0/docs/_build/html/_static/plus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.6.0/docs/authors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6406 2023-06-18 10:02:01.000000 jaxip-0.6.0/docs/conf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.6.0/docs/contributing.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       71 2023-05-17 19:30:18.000000 jaxip-0.6.0/docs/examples.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.6.0/docs/history.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.357491 jaxip-0.6.0/docs/images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.6.0/docs/images/flowchart.drawio.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.6.0/docs/images/water.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      315 2023-05-06 13:11:44.000000 jaxip-0.6.0/docs/index.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.6.0/docs/installation.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-05-10 20:36:05.000000 jaxip-0.6.0/docs/jaxip.atoms.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      662 2023-05-17 19:30:18.000000 jaxip-0.6.0/docs/jaxip.datasets.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-05-10 20:36:05.000000 jaxip-0.6.0/docs/jaxip.descriptors.acsf.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      613 2023-05-17 19:30:18.000000 jaxip-0.6.0/docs/jaxip.descriptors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-05-10 20:36:05.000000 jaxip-0.6.0/docs/jaxip.models.nn.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      400 2023-05-17 19:30:18.000000 jaxip-0.6.0/docs/jaxip.models.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1290 2023-05-17 19:30:18.000000 jaxip-0.6.0/docs/jaxip.potentials.nnp.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      464 2023-05-10 20:36:05.000000 jaxip-0.6.0/docs/jaxip.potentials.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      961 2023-06-18 10:02:01.000000 jaxip-0.6.0/docs/jaxip.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      560 2023-06-18 10:02:01.000000 jaxip-0.6.0/docs/jaxip.simulation.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-05-10 20:36:05.000000 jaxip-0.6.0/docs/jaxip.utils.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.6.0/docs/make.bat
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-06-18 09:19:55.000000 jaxip-0.6.0/docs/modules.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.6.0/docs/readme.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-06 13:11:44.000000 jaxip-0.6.0/docs/theory.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.6.0/docs/usage.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.365491 jaxip-0.6.0/jaxip/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      575 2023-05-06 13:11:44.000000 jaxip-0.6.0/jaxip/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-06-18 10:02:01.000000 jaxip-0.6.0/jaxip/_version.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.369491 jaxip-0.6.0/jaxip/atoms/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      174 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/atoms/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      355 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/atoms/_box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      779 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/atoms/_neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1342 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/atoms/_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3918 2023-06-18 10:02:01.000000 jaxip-0.6.0/jaxip/atoms/box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6639 2023-06-18 10:02:01.000000 jaxip-0.6.0/jaxip/atoms/element.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3015 2023-05-09 21:10:18.000000 jaxip-0.6.0/jaxip/atoms/neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    17216 2023-06-18 10:02:01.000000 jaxip-0.6.0/jaxip/atoms/structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1131 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/config.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.369491 jaxip-0.6.0/jaxip/datasets/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      154 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/datasets/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      408 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/datasets/dataset.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6445 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/datasets/runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1039 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/datasets/transformer.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.373491 jaxip-0.6.0/jaxip/descriptors/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/descriptors/__init__.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.373491 jaxip-0.6.0/jaxip/descriptors/acsf/
--rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.6.0/jaxip/descriptors/acsf/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5275 2023-05-06 13:11:44.000000 jaxip-0.6.0/jaxip/descriptors/acsf/_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7689 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/descriptors/acsf/acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2236 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/descriptors/acsf/angular.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2627 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/descriptors/acsf/cutoff.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1495 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/descriptors/acsf/radial.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1015 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/descriptors/acsf/symmetry.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      616 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/descriptors/descriptor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7476 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/descriptors/scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/logger.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.373491 jaxip-0.6.0/jaxip/models/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       88 2023-05-08 16:51:03.000000 jaxip-0.6.0/jaxip/models/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      389 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/models/model.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.373491 jaxip-0.6.0/jaxip/models/nn/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      181 2023-05-08 16:51:03.000000 jaxip-0.6.0/jaxip/models/nn/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-08 16:51:03.000000 jaxip-0.6.0/jaxip/models/nn/activation.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-05-08 16:51:03.000000 jaxip-0.6.0/jaxip/models/nn/initializer.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2911 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/models/nn/network.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.373491 jaxip-0.6.0/jaxip/potentials/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      212 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1973 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/_energy.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/potentials/_force.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1831 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/atomic_potential.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.377491 jaxip-0.6.0/jaxip/potentials/nnp/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      238 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/nnp/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9155 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/nnp/gradient_descent.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9364 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/nnp/kalman_filter.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/potentials/nnp/metrics.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      545 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/nnp/nnp.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    18966 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/nnp/potential.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11352 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/nnp/settings.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3585 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/pytree.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.377491 jaxip-0.6.0/jaxip/simulation/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      163 2023-06-18 10:02:01.000000 jaxip-0.6.0/jaxip/simulation/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     8913 2023-06-18 10:02:01.000000 jaxip-0.6.0/jaxip/simulation/md.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      832 2023-06-18 10:02:01.000000 jaxip-0.6.0/jaxip/simulation/thermostat.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      643 2023-05-07 09:13:07.000000 jaxip-0.6.0/jaxip/types.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2573 2023-06-18 10:02:01.000000 jaxip-0.6.0/jaxip/units.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.377491 jaxip-0.6.0/jaxip/utils/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/utils/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1427 2023-02-18 20:52:11.000000 jaxip-0.6.0/jaxip/utils/attribute.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/utils/batch.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2008 2023-03-23 20:22:06.000000 jaxip-0.6.0/jaxip/utils/compare.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/utils/profiler.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.6.0/jaxip/utils/tokenize.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.369491 jaxip-0.6.0/jaxip.egg-info/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5332 2023-06-18 10:02:54.000000 jaxip-0.6.0/jaxip.egg-info/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3217 2023-06-18 10:02:54.000000 jaxip-0.6.0/jaxip.egg-info/SOURCES.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-06-18 10:02:54.000000 jaxip-0.6.0/jaxip.egg-info/dependency_links.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-06-18 10:02:54.000000 jaxip-0.6.0/jaxip.egg-info/entry_points.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-06-18 10:02:54.000000 jaxip-0.6.0/jaxip.egg-info/not-zip-safe
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-06-18 10:02:54.000000 jaxip-0.6.0/jaxip.egg-info/requires.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-06-18 10:02:54.000000 jaxip-0.6.0/jaxip.egg-info/top_level.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-06-18 10:02:54.385491 jaxip-0.6.0/setup.cfg
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.6.0/setup.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.381492 jaxip-0.6.0/tests/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.381492 jaxip-0.6.0/tests/.ipynb_checkpoints/
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.6.0/tests/.ipynb_checkpoints/h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.6.0/tests/.ipynb_checkpoints/h2o-checkpoint.json
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.6.0/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.6.0/tests/.ipynb_checkpoints/test-checkpoint.ipynb
--rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.6.0/tests/__init__.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.6.0/tests/h2o.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.6.0/tests/h2o.json
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-06-18 09:42:24.000000 jaxip-0.6.0/tests/scaling.001.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-06-18 09:42:24.000000 jaxip-0.6.0/tests/scaling.008.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5117 2023-05-07 11:23:30.000000 jaxip-0.6.0/tests/test_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4858 2023-06-18 10:02:01.000000 jaxip-0.6.0/tests/test_md.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4116 2023-05-08 16:51:03.000000 jaxip-0.6.0/tests/test_nn.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3472 2023-05-17 19:30:18.000000 jaxip-0.6.0/tests/test_nnp.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4816 2023-05-01 12:41:07.000000 jaxip-0.6.0/tests/test_runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2859 2023-05-01 12:41:07.000000 jaxip-0.6.0/tests/test_scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5463 2023-06-18 10:02:01.000000 jaxip-0.6.0/tests/test_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-06-18 09:42:24.000000 jaxip-0.6.0/tests/weights.001.pkl
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-06-18 09:42:24.000000 jaxip-0.6.0/tests/weights.008.pkl
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.908974 jaxip-0.6.1/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.6.1/AUTHORS.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.6.1/CONTRIBUTING.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      669 2023-06-24 19:26:34.000000 jaxip-0.6.1/HISTORY.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.6.1/LICENSE
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.6.1/MANIFEST.in
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5332 2023-06-24 19:26:59.908974 jaxip-0.6.1/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4745 2023-05-17 19:30:18.000000 jaxip-0.6.1/README.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.864973 jaxip-0.6.1/docs/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.6.1/docs/Makefile
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.856973 jaxip-0.6.1/docs/_build/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.856973 jaxip-0.6.1/docs/_build/doctrees/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.864973 jaxip-0.6.1/docs/_build/doctrees/nbsphinx/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-06-18 09:34:19.000000 jaxip-0.6.1/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-06-18 09:34:19.000000 jaxip-0.6.1/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-06-18 09:34:19.000000 jaxip-0.6.1/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.856973 jaxip-0.6.1/docs/_build/html/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.868973 jaxip-0.6.1/docs/_build/html/_images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-06-18 09:20:05.000000 jaxip-0.6.1/docs/_build/html/_images/notebooks_tutorials_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-06-18 09:20:05.000000 jaxip-0.6.1/docs/_build/html/_images/notebooks_tutorials_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-06-18 09:20:05.000000 jaxip-0.6.1/docs/_build/html/_images/notebooks_tutorials_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.872973 jaxip-0.6.1/docs/_build/html/_static/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.6.1/docs/_build/html/_static/file.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.6.1/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.6.1/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.6.1/docs/authors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6406 2023-06-18 10:02:01.000000 jaxip-0.6.1/docs/conf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.6.1/docs/contributing.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       71 2023-05-17 19:30:18.000000 jaxip-0.6.1/docs/examples.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.6.1/docs/history.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.880973 jaxip-0.6.1/docs/images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.6.1/docs/images/flowchart.drawio.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.6.1/docs/images/water.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      315 2023-05-06 13:11:44.000000 jaxip-0.6.1/docs/index.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.6.1/docs/installation.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-05-10 20:36:05.000000 jaxip-0.6.1/docs/jaxip.atoms.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      662 2023-05-17 19:30:18.000000 jaxip-0.6.1/docs/jaxip.datasets.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-05-10 20:36:05.000000 jaxip-0.6.1/docs/jaxip.descriptors.acsf.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      613 2023-05-17 19:30:18.000000 jaxip-0.6.1/docs/jaxip.descriptors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-05-10 20:36:05.000000 jaxip-0.6.1/docs/jaxip.models.nn.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      400 2023-05-17 19:30:18.000000 jaxip-0.6.1/docs/jaxip.models.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1290 2023-05-17 19:30:18.000000 jaxip-0.6.1/docs/jaxip.potentials.nnp.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      464 2023-05-10 20:36:05.000000 jaxip-0.6.1/docs/jaxip.potentials.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      961 2023-06-18 10:02:01.000000 jaxip-0.6.1/docs/jaxip.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      560 2023-06-18 10:02:01.000000 jaxip-0.6.1/docs/jaxip.simulation.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-05-10 20:36:05.000000 jaxip-0.6.1/docs/jaxip.utils.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.6.1/docs/make.bat
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-06-18 09:19:55.000000 jaxip-0.6.1/docs/modules.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.6.1/docs/readme.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-06 13:11:44.000000 jaxip-0.6.1/docs/theory.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.6.1/docs/usage.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.884973 jaxip-0.6.1/jaxip/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      575 2023-05-06 13:11:44.000000 jaxip-0.6.1/jaxip/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/_version.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.888973 jaxip-0.6.1/jaxip/atoms/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      174 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/atoms/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      355 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/atoms/_box.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      779 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/atoms/_neighbor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1471 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/atoms/_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3918 2023-06-18 10:02:01.000000 jaxip-0.6.1/jaxip/atoms/box.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6639 2023-06-18 10:02:01.000000 jaxip-0.6.1/jaxip/atoms/element.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3015 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/atoms/neighbor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    17266 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/atoms/structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1131 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/config.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.888973 jaxip-0.6.1/jaxip/datasets/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      154 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/datasets/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      408 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/datasets/dataset.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6445 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/datasets/runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1039 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/datasets/transformer.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.892974 jaxip-0.6.1/jaxip/descriptors/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/descriptors/__init__.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.892974 jaxip-0.6.1/jaxip/descriptors/acsf/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.6.1/jaxip/descriptors/acsf/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5275 2023-05-06 13:11:44.000000 jaxip-0.6.1/jaxip/descriptors/acsf/_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7767 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/descriptors/acsf/acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2236 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/descriptors/acsf/angular.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2627 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/descriptors/acsf/cutoff.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1495 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/descriptors/acsf/radial.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1015 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/descriptors/acsf/symmetry.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      616 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/descriptors/descriptor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7476 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/descriptors/scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/logger.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.892974 jaxip-0.6.1/jaxip/models/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       88 2023-05-08 16:51:03.000000 jaxip-0.6.1/jaxip/models/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      389 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/models/model.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.892974 jaxip-0.6.1/jaxip/models/nn/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      181 2023-05-08 16:51:03.000000 jaxip-0.6.1/jaxip/models/nn/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-08 16:51:03.000000 jaxip-0.6.1/jaxip/models/nn/activation.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-05-08 16:51:03.000000 jaxip-0.6.1/jaxip/models/nn/initializer.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2911 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/models/nn/network.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.892974 jaxip-0.6.1/jaxip/potentials/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      212 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/potentials/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1973 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/potentials/_energy.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/potentials/_force.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1831 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/potentials/atomic_potential.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.892974 jaxip-0.6.1/jaxip/potentials/nnp/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      238 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/potentials/nnp/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9149 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/potentials/nnp/gradient_descent.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9358 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/potentials/nnp/kalman_filter.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/potentials/nnp/metrics.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      542 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/potentials/nnp/nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    18963 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/potentials/nnp/potential.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11352 2023-06-22 07:40:24.000000 jaxip-0.6.1/jaxip/potentials/nnp/settings.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3585 2023-05-17 19:30:18.000000 jaxip-0.6.1/jaxip/pytree.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.896973 jaxip-0.6.1/jaxip/simulation/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      296 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/simulation/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4289 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/simulation/mc.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     8395 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/simulation/md.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1756 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/simulation/run.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      834 2023-06-24 19:26:34.000000 jaxip-0.6.1/jaxip/simulation/thermostat.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      643 2023-05-07 09:13:07.000000 jaxip-0.6.1/jaxip/types.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2573 2023-06-18 10:02:01.000000 jaxip-0.6.1/jaxip/units.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.896973 jaxip-0.6.1/jaxip/utils/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/utils/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1427 2023-02-18 20:52:11.000000 jaxip-0.6.1/jaxip/utils/attribute.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/utils/batch.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2008 2023-03-23 20:22:06.000000 jaxip-0.6.1/jaxip/utils/compare.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.6.1/jaxip/utils/profiler.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.6.1/jaxip/utils/tokenize.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.888973 jaxip-0.6.1/jaxip.egg-info/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5332 2023-06-24 19:26:59.000000 jaxip-0.6.1/jaxip.egg-info/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3296 2023-06-24 19:26:59.000000 jaxip-0.6.1/jaxip.egg-info/SOURCES.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-06-24 19:26:59.000000 jaxip-0.6.1/jaxip.egg-info/dependency_links.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-06-24 19:26:59.000000 jaxip-0.6.1/jaxip.egg-info/entry_points.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-06-22 10:45:16.000000 jaxip-0.6.1/jaxip.egg-info/not-zip-safe
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-06-24 19:26:59.000000 jaxip-0.6.1/jaxip.egg-info/requires.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-06-24 19:26:59.000000 jaxip-0.6.1/jaxip.egg-info/top_level.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-06-24 19:26:59.908974 jaxip-0.6.1/setup.cfg
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.6.1/setup.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.900973 jaxip-0.6.1/tests/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-24 19:26:59.904974 jaxip-0.6.1/tests/.ipynb_checkpoints/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.6.1/tests/.ipynb_checkpoints/h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.6.1/tests/.ipynb_checkpoints/h2o-checkpoint.json
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.6.1/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.6.1/tests/.ipynb_checkpoints/test-checkpoint.ipynb
+-rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.6.1/tests/__init__.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.6.1/tests/h2o.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.6.1/tests/h2o.json
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1681 2023-06-24 19:26:34.000000 jaxip-0.6.1/tests/ljpot.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-06-24 19:18:13.000000 jaxip-0.6.1/tests/scaling.001.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-06-24 19:18:13.000000 jaxip-0.6.1/tests/scaling.008.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5116 2023-06-24 19:26:34.000000 jaxip-0.6.1/tests/test_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2536 2023-06-24 19:26:34.000000 jaxip-0.6.1/tests/test_mc.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3242 2023-06-24 19:26:34.000000 jaxip-0.6.1/tests/test_md.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4115 2023-06-24 19:26:34.000000 jaxip-0.6.1/tests/test_nn.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3469 2023-06-24 19:26:34.000000 jaxip-0.6.1/tests/test_nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4816 2023-05-01 12:41:07.000000 jaxip-0.6.1/tests/test_runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2859 2023-05-01 12:41:07.000000 jaxip-0.6.1/tests/test_scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5465 2023-06-24 19:26:34.000000 jaxip-0.6.1/tests/test_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-06-24 19:18:13.000000 jaxip-0.6.1/tests/weights.001.pkl
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-06-24 19:18:13.000000 jaxip-0.6.1/tests/weights.008.pkl
```

### Comparing `jaxip-0.6.0/CONTRIBUTING.rst` & `jaxip-0.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/LICENSE` & `jaxip-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/PKG-INFO` & `jaxip-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxip
-Version: 0.6.0
+Version: 0.6.1
 Summary: JAX-based Interatomic Potential
 Home-page: https://github.com/hghcomphys/jaxip
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: jaxip
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `jaxip-0.6.0/README.rst` & `jaxip-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/Makefile` & `jaxip-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png` & `jaxip-0.6.1/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png` & `jaxip-0.6.1/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png` & `jaxip-0.6.1/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/_build/html/_images/notebooks_tutorials_38_0.png` & `jaxip-0.6.1/docs/_build/html/_images/notebooks_tutorials_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/_build/html/_images/notebooks_tutorials_45_0.png` & `jaxip-0.6.1/docs/_build/html/_images/notebooks_tutorials_45_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/_build/html/_images/notebooks_tutorials_51_0.png` & `jaxip-0.6.1/docs/_build/html/_images/notebooks_tutorials_51_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/conf.py` & `jaxip-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/images/flowchart.drawio.png` & `jaxip-0.6.1/docs/images/flowchart.drawio.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/images/water.png` & `jaxip-0.6.1/docs/images/water.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/installation.rst` & `jaxip-0.6.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/jaxip.atoms.rst` & `jaxip-0.6.1/docs/jaxip.atoms.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/jaxip.datasets.rst` & `jaxip-0.6.1/docs/jaxip.datasets.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/jaxip.descriptors.acsf.rst` & `jaxip-0.6.1/docs/jaxip.descriptors.acsf.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/jaxip.descriptors.rst` & `jaxip-0.6.1/docs/jaxip.descriptors.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/jaxip.models.nn.rst` & `jaxip-0.6.1/docs/jaxip.models.nn.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/jaxip.potentials.nnp.rst` & `jaxip-0.6.1/docs/jaxip.potentials.nnp.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/jaxip.rst` & `jaxip-0.6.1/docs/jaxip.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/jaxip.simulation.rst` & `jaxip-0.6.1/docs/jaxip.simulation.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/jaxip.utils.rst` & `jaxip-0.6.1/docs/jaxip.utils.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/make.bat` & `jaxip-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/theory.rst` & `jaxip-0.6.1/docs/theory.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/docs/usage.rst` & `jaxip-0.6.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/__init__.py` & `jaxip-0.6.1/jaxip/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/atoms/_neighbor.py` & `jaxip-0.6.1/jaxip/atoms/_neighbor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/atoms/_structure.py` & `jaxip-0.6.1/jaxip/atoms/_structure.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,7 +40,12 @@
 def _calculate_distance(
     atom_position: Array,
     neighbor_position: Array,
     lattice: Optional[Array] = None,
 ) -> Tuple[Array, Array]:
     """Calculate an array of distances between multiple atoms and the neighbors (using `jax.vmap`)."""
     return _vmap_calculate_distance(atom_position, neighbor_position, lattice)
+
+
+@jax.jit
+def _get_center_of_mass(array: Array, mass: Array) -> Array:
+    return jnp.sum(mass * array, axis=0) / jnp.sum(mass)
```

### Comparing `jaxip-0.6.0/jaxip/atoms/box.py` & `jaxip-0.6.1/jaxip/atoms/box.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/atoms/element.py` & `jaxip-0.6.1/jaxip/atoms/element.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/atoms/neighbor.py` & `jaxip-0.6.1/jaxip/atoms/neighbor.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     r_cutoff: Optional[float] = None
     r_cutoff_updated: bool = field(init=False, default=False)
 
     def __post_init__(self) -> None:
         """Post initialize the neighbor list."""
         logger.debug(f"Initializing {self}")
         self._assert_jit_dynamic_attributes(expected=("mask",))
-        self._assert_jit_static_attributes(expected=('r_cutoff', 'r_cutoff_updated'))
+        self._assert_jit_static_attributes(expected=("r_cutoff", "r_cutoff_updated"))
 
     def __hash__(self) -> int:
         """Enforce to use the parent class's hash method (JIT)."""
         return super().__hash__()
 
     def set_cutoff_radius(self, r_cutoff: float) -> None:
         """
```

### Comparing `jaxip-0.6.0/jaxip/atoms/structure.py` & `jaxip-0.6.1/jaxip/atoms/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from dataclasses import dataclass, field
-from functools import cached_property
 from typing import Any, DefaultDict, Dict, Generator, List, NamedTuple, Optional, Tuple
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 from ase import Atoms as AseAtoms
 from jax import tree_util
 
-from jaxip.atoms._structure import _calculate_distance
+from jaxip.atoms._structure import _calculate_distance, _get_center_of_mass
 from jaxip.atoms.box import Box
 from jaxip.atoms.element import ElementMap
 from jaxip.atoms.neighbor import Neighbor
 from jaxip.logger import logger
 from jaxip.pytree import BaseJaxPytreeDataClass, register_jax_pytree_node
 from jaxip.types import Array, Dtype, Element
 from jaxip.types import dtype as _dtype
@@ -309,17 +308,15 @@
 
     @property
     def mass(self) -> Array:
         """Return an array of atomic masses."""
         to_element = self.element_map.atom_type_to_element
         elements = (to_element[int(at)] for at in self.atom_type)
         return jnp.array(
-            tuple(
-                ElementMap.element_to_atomic_mass(element) for element in elements
-            )
+            tuple(ElementMap.element_to_atomic_mass(element) for element in elements)
         )
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}"
             f"(natoms={self.natoms}, elements={self.elements}, dtype={self.dtype})"
         )
@@ -329,15 +326,15 @@
         Return all atom indices of the element.
 
         :param element: element name (e.g. `H` for hydrogen)
         :return: atom indices
         """
         return jnp.nonzero(self.atom_type == self.element_map[element])[0]
 
-    @jax.jit
+    # @jax.jit
     def calculate_distance(
         self,
         atom_index: Array,
         neighbor_index: Optional[Array] = None,
     ) -> Tuple[Array, Array]:
         """
         Calculate distances between specific atoms (given by atom indices)
@@ -391,20 +388,16 @@
 
         :return: ASE representation of the structure
         :rtype: AseAtoms
         """
         logger.info("Creating a representation of the structure in form of ASE atoms")
         return AseAtoms(
             symbols=[self.element_map(int(at)) for at in self.atom_type],
-            positions=[
-                units.TO_ANGSTROM * np.asarray(pos) for pos in self.position
-            ],
-            cell=units.TO_ANGSTROM * np.asarray(self.box.lattice)
-            if self.box
-            else None,
+            positions=[units.TO_ANGSTROM * np.asarray(pos) for pos in self.position],
+            cell=units.TO_ANGSTROM * np.asarray(self.box.lattice) if self.box else None,
             pbc=True if self.box else False,
             charges=[np.asarray(ch) for ch in self.charge],
         )
 
     # --------------------------------------------------------------------------------------
 
     def _get_energy_offset(self, atom_energy: Dict[Element, float]) -> Array:
@@ -433,14 +426,18 @@
 
         :param atom_energy: atom reference energy
         """
         energy_offset = self._get_energy_offset(atom_energy)
         self.energy += energy_offset
         self.total_energy += energy_offset.sum()
 
+    def get_com_position(self) -> Array:
+        """Return center of mass position."""
+        return _get_center_of_mass(self.position, self.mass)
+
     # --------------------------------------------------------------------------------------
 
     def get_inputs(self) -> Dict[Element, Inputs]:
         """A tuple of required info which are used for training and evaluating the potential."""
 
         def extract_input() -> Generator[Tuple[Element, Inputs], None, None]:
             for element in self.elements:
```

### Comparing `jaxip-0.6.0/jaxip/config.py` & `jaxip-0.6.1/jaxip/config.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/datasets/runner.py` & `jaxip-0.6.1/jaxip/datasets/runner.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/datasets/transformer.py` & `jaxip-0.6.1/jaxip/datasets/transformer.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/descriptors/acsf/_acsf.py` & `jaxip-0.6.1/jaxip/descriptors/acsf/_acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/descriptors/acsf/acsf.py` & `jaxip-0.6.1/jaxip/descriptors/acsf/acsf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import itertools
 from dataclasses import dataclass
 from typing import Optional, Tuple
 
 import jax.numpy as jnp
 
 from jaxip.atoms.structure import Structure
-from jaxip.descriptors.acsf._acsf import (
-    _calculate_descriptor,
-    _calculate_grad_descriptor_per_atom,
-)
+from jaxip.descriptors.acsf._acsf import (_calculate_descriptor,
+                                          _calculate_grad_descriptor_per_atom)
 from jaxip.descriptors.acsf.angular import AngularSymmetryFunction
 from jaxip.descriptors.acsf.radial import RadialSymmetryFunction
-from jaxip.descriptors.acsf.symmetry import BaseSymmetryFunction, EnvironmentElements
+from jaxip.descriptors.acsf.symmetry import (BaseSymmetryFunction,
+                                             EnvironmentElements)
 from jaxip.descriptors.descriptor import DescriptorInterface
 from jaxip.logger import logger
 from jaxip.pytree import BaseJaxPytreeDataClass, register_jax_pytree_node
 from jaxip.types import Array, Element
 
 
 @dataclass
```

### Comparing `jaxip-0.6.0/jaxip/descriptors/acsf/angular.py` & `jaxip-0.6.1/jaxip/descriptors/acsf/angular.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/descriptors/acsf/cutoff.py` & `jaxip-0.6.1/jaxip/descriptors/acsf/cutoff.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/descriptors/acsf/radial.py` & `jaxip-0.6.1/jaxip/descriptors/acsf/radial.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/descriptors/acsf/symmetry.py` & `jaxip-0.6.1/jaxip/descriptors/acsf/symmetry.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/descriptors/descriptor.py` & `jaxip-0.6.1/jaxip/descriptors/descriptor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/descriptors/scaler.py` & `jaxip-0.6.1/jaxip/descriptors/scaler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/logger.py` & `jaxip-0.6.1/jaxip/logger.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/models/nn/activation.py` & `jaxip-0.6.1/jaxip/models/nn/activation.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/models/nn/initializer.py` & `jaxip-0.6.1/jaxip/models/nn/initializer.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/models/nn/network.py` & `jaxip-0.6.1/jaxip/models/nn/network.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/potentials/_energy.py` & `jaxip-0.6.1/jaxip/potentials/_energy.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/potentials/_force.py` & `jaxip-0.6.1/jaxip/potentials/_force.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/potentials/atomic_potential.py` & `jaxip-0.6.1/jaxip/potentials/atomic_potential.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/potentials/nnp/gradient_descent.py` & `jaxip-0.6.1/jaxip/potentials/nnp/gradient_descent.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,18 @@
 
 from jaxip.atoms.structure import Structure
 from jaxip.datasets.dataset import DatasetInterface
 from jaxip.logger import logger
 from jaxip.potentials._energy import _energy_fn
 from jaxip.potentials._force import _compute_force
 from jaxip.potentials.nnp.metrics import ErrorMetric
-from jaxip.potentials.nnp.nnp import (
-    NeuralNetworkPotentialInterface as PotentialInterface,
-)
-from jaxip.potentials.nnp.settings import (
-    NeuralNetworkPotentialSettings as PotentialSettings,
-)
+from jaxip.potentials.nnp.nnp import \
+    NeuralNetworkPotentialInterface as PotentialInterface
+from jaxip.potentials.nnp.settings import \
+    NeuralNetworkPotentialSettings as PotentialSettings
 from jaxip.types import Array, Element
 
 
 def _mse_loss(*, logits: Array, targets: Array) -> Array:
     return ((targets - logits) ** 2).mean()
```

### Comparing `jaxip-0.6.0/jaxip/potentials/nnp/kalman_filter.py` & `jaxip-0.6.1/jaxip/potentials/nnp/kalman_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 
 from jaxip.atoms.structure import Structure
 from jaxip.datasets.dataset import DatasetInterface
 from jaxip.logger import logger
 from jaxip.potentials._energy import _compute_energy
 from jaxip.potentials._force import _compute_force
 from jaxip.potentials.atomic_potential import AtomicPotential
-from jaxip.potentials.nnp.nnp import (
-    NeuralNetworkPotentialInterface as PotentialInterface,
-)
-from jaxip.potentials.nnp.settings import (
-    NeuralNetworkPotentialSettings as PotentialSettings,
-)
+from jaxip.potentials.nnp.nnp import \
+    NeuralNetworkPotentialInterface as PotentialInterface
+from jaxip.potentials.nnp.settings import \
+    NeuralNetworkPotentialSettings as PotentialSettings
 from jaxip.types import Array, Element
 from jaxip.types import dtype as default_dtype
 
 
 def _tree_flatten(pytree: Dict) -> Array:
     return flatten_util.ravel_pytree(pytree)[0].reshape(-1, 1)  # type: ignore
```

### Comparing `jaxip-0.6.0/jaxip/potentials/nnp/metrics.py` & `jaxip-0.6.1/jaxip/potentials/nnp/metrics.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/potentials/nnp/nnp.py` & `jaxip-0.6.1/jaxip/potentials/nnp/nnp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Dict, Protocol, Tuple
 
 from frozendict import frozendict
 
 from jaxip.potentials.atomic_potential import AtomicPotential
-from jaxip.potentials.nnp.settings import (
-    NeuralNetworkPotentialSettings as PotentialSettings,
-)
+from jaxip.potentials.nnp.settings import \
+    NeuralNetworkPotentialSettings as PotentialSettings
 from jaxip.types import Element
 
 
 class NeuralNetworkPotentialInterface(Protocol):
     """Interface for neural network potential (NNP)."""
 
     settings: PotentialSettings
```

### Comparing `jaxip-0.6.0/jaxip/potentials/nnp/potential.py` & `jaxip-0.6.1/jaxip/potentials/nnp/potential.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,16 @@
 from jaxip.models.nn.initializer import UniformInitializer
 from jaxip.models.nn.network import NeuralNetworkModel
 from jaxip.potentials._energy import _compute_energy
 from jaxip.potentials._force import _compute_force
 from jaxip.potentials.atomic_potential import AtomicPotential
 from jaxip.potentials.nnp.gradient_descent import GradientDescentUpdater
 from jaxip.potentials.nnp.kalman_filter import KalmanFilterUpdater
-from jaxip.potentials.nnp.settings import (
-    NeuralNetworkPotentialSettings as PotentialSettings,
-)
+from jaxip.potentials.nnp.settings import \
+    NeuralNetworkPotentialSettings as PotentialSettings
 from jaxip.types import Array, Element
 
 
 class UpdaterInterface(Protocol):
     """Interface for potential weight updaters."""
 
     def fit(self, dataset: DatasetInterface) -> Dict:
```

### Comparing `jaxip-0.6.0/jaxip/potentials/nnp/settings.py` & `jaxip-0.6.1/jaxip/potentials/nnp/settings.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/pytree.py` & `jaxip-0.6.1/jaxip/pytree.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/simulation/md.py` & `jaxip-0.6.1/jaxip/simulation/md.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import replace
 from typing import Optional, Protocol, Tuple
 
 import jax
 import jax.numpy as jnp
 
 from jaxip.atoms import Structure
+from jaxip.atoms._structure import _get_center_of_mass
 from jaxip.logger import logger
 from jaxip.simulation.thermostat import BrendsenThermostat
 from jaxip.types import Array, Element
 from jaxip.units import units
 
 KB = units.BOLTZMANN_CONSTANT
 
@@ -18,19 +19,14 @@
         ...
 
     def compute_force(self, structure: Structure) -> Array:
         ...
 
 
 @jax.jit
-def _get_center_of_mass(array: Array, mass: Array) -> Array:
-    return jnp.sum(mass * array, axis=0) / jnp.sum(mass)
-
-
-@jax.jit
 def _get_kinetic_energy(velocity: Array, mass: Array) -> Array:
     return 0.5 * jnp.sum(mass * velocity * velocity)
 
 
 @jax.jit
 def _get_temperature(velocity: Array, mass: Array) -> Array:
     kinetic_energy = _get_kinetic_energy(velocity, mass)
@@ -135,42 +131,23 @@
 
         self.step: int = 0
         self.elapsed_time: float = 0.0
         self.force = _compute_force(self.potential, initial_structure)
         self.temperature = _get_temperature(self.velocity, self.mass)
         self._structure = replace(initial_structure)
 
-    def run_simulation(
-        self,
-        num_steps: int = 1,
-        output_freq: Optional[int] = None,
-    ) -> None:
-        """Run molecular simulation for a given number of steps."""
-        if output_freq is None:
-            output_freq = 1 if num_steps < 100 else int(0.01 * num_steps)
-        is_output = output_freq > 0
-        init_step = self.step
-        try:
-            for _ in range(num_steps):
-                if is_output and ((self.step - init_step) % output_freq == 0):
-                    print(self.repr_physical_params())
-                self.molecular_dynamics_step()
-        except KeyboardInterrupt:
-            print("KeyboardInterrupt")
-        if is_output:
-            print(self.repr_physical_params())
-
-    def molecular_dynamics_step(self) -> None:
+    def update(self) -> None:
         """Update parameters for next time step."""
         self.verlet_integration()
         self.step += 1
         self.elapsed_time += self.time_step
         self.temperature = _get_temperature(self.velocity, self.mass)
         if self.thermostat is not None:
             self.velocity = self.thermostat.get_rescaled_velocity(self)
+            self.temperature = _get_temperature(self.velocity, self.mass)
 
     def verlet_integration(self) -> None:
         """Update atom positions and velocities based on Verlet algorithm."""
         new_position = (
             self.position
             + self.velocity * self.time_step
             + 0.5 * self.force * self.time_step * self.time_step
@@ -193,20 +170,24 @@
         natoms = mass.shape[0]
         velocity = jax.random.normal(key, shape=(natoms, 3))
         velocity *= jnp.sqrt(temperature / _get_temperature(velocity, mass))
         velocity -= _get_center_of_mass(velocity, mass)
         return velocity
 
     def repr_physical_params(self) -> str:
+        """Represent current physical parameters."""
         return (
             f"{self.step:<10} "
             f"time[ps]:{units.TO_PICO_SECOND * self.elapsed_time:<10.5f} "
-            f"Temp[K]:{self.temperature:<15.10f} "
+            f"Temp[K]:{self.temperature:<10.5f} "
             f"Etot[Ha]:{self.get_total_energy():<15.10f} "
             f"Epot[Ha]:{self.get_potential_energy():<15.10f} "
+            f"Pres[kb]:{self.get_pressure() * units.TO_KILO_BAR:<10.5f}"
+            if self._structure.box
+            else ""
         )
 
     @property
     def position(self) -> Array:
         return self._structure.position
 
     @property
@@ -225,15 +206,20 @@
         )
 
     def get_pressure(self) -> Array:
         assert (
             self._structure.box
         ), "Calulating pressure... input structure must have PBC box"
         volume = self._structure.box.volume
-        virial = _get_virial_term(self.velocity, self.mass, self.position, self.force)
+        virial = _get_virial_term(
+            self.velocity,
+            self.mass,
+            self.position,
+            self.force,
+        )
         return virial / (3.0 * volume)  # type: ignore
 
     def get_com_velocity(self) -> Array:
         """Return center of mass velocity."""
         return _get_center_of_mass(self.velocity, self.mass)
 
     def get_com_position(self) -> Array:
```

### Comparing `jaxip-0.6.0/jaxip/simulation/thermostat.py` & `jaxip-0.6.1/jaxip/simulation/thermostat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from jaxip.types import Array
-import jax.numpy as jnp
 from typing import Protocol
 
+import jax.numpy as jnp
+
+from jaxip.types import Array
+
 
 class MDSimulatorInterface(Protocol):
     temperature: float
     time_step: float
     velocity: Array
```

### Comparing `jaxip-0.6.0/jaxip/types.py` & `jaxip-0.6.1/jaxip/types.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/units.py` & `jaxip-0.6.1/jaxip/units.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/utils/attribute.py` & `jaxip-0.6.1/jaxip/utils/attribute.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/utils/batch.py` & `jaxip-0.6.1/jaxip/utils/batch.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/utils/compare.py` & `jaxip-0.6.1/jaxip/utils/compare.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/utils/profiler.py` & `jaxip-0.6.1/jaxip/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip/utils/tokenize.py` & `jaxip-0.6.1/jaxip/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/jaxip.egg-info/PKG-INFO` & `jaxip-0.6.1/jaxip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxip
-Version: 0.6.0
+Version: 0.6.1
 Summary: JAX-based Interatomic Potential
 Home-page: https://github.com/hghcomphys/jaxip
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: jaxip
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `jaxip-0.6.0/jaxip.egg-info/SOURCES.txt` & `jaxip-0.6.1/jaxip.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -91,28 +91,32 @@
 jaxip/potentials/nnp/gradient_descent.py
 jaxip/potentials/nnp/kalman_filter.py
 jaxip/potentials/nnp/metrics.py
 jaxip/potentials/nnp/nnp.py
 jaxip/potentials/nnp/potential.py
 jaxip/potentials/nnp/settings.py
 jaxip/simulation/__init__.py
+jaxip/simulation/mc.py
 jaxip/simulation/md.py
+jaxip/simulation/run.py
 jaxip/simulation/thermostat.py
 jaxip/utils/__init__.py
 jaxip/utils/attribute.py
 jaxip/utils/batch.py
 jaxip/utils/compare.py
 jaxip/utils/profiler.py
 jaxip/utils/tokenize.py
 tests/__init__.py
 tests/h2o.data
 tests/h2o.json
+tests/ljpot.py
 tests/scaling.001.data
 tests/scaling.008.data
 tests/test_acsf.py
+tests/test_mc.py
 tests/test_md.py
 tests/test_nn.py
 tests/test_nnp.py
 tests/test_runner.py
 tests/test_scaler.py
 tests/test_structure.py
 tests/weights.001.pkl
```

### Comparing `jaxip-0.6.0/setup.py` & `jaxip-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/tests/.ipynb_checkpoints/h2o-checkpoint.data` & `jaxip-0.6.1/tests/.ipynb_checkpoints/h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/tests/.ipynb_checkpoints/h2o-checkpoint.json` & `jaxip-0.6.1/tests/.ipynb_checkpoints/h2o-checkpoint.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/tests/.ipynb_checkpoints/input.h2o-checkpoint.data` & `jaxip-0.6.1/tests/.ipynb_checkpoints/input.h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/tests/.ipynb_checkpoints/test-checkpoint.ipynb` & `jaxip-0.6.1/tests/.ipynb_checkpoints/test-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/tests/h2o.data` & `jaxip-0.6.1/tests/h2o.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/tests/h2o.json` & `jaxip-0.6.1/tests/h2o.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/tests/test_acsf.py` & `jaxip-0.6.1/tests/test_acsf.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
                 ),
             ),
         ),
     )
 
 
 class TestACSF:
-
     lj_structure: Structure = Structure.create_from_dict(
         {
             "position": [[0.0, 0.0, 0.0], [0.588897275, 0.588897275, 0.588897275]],
             "element": ["Ne", "Ne"],
         }
     )
     h2o_structure: Structure = Structure.create_from_dict(
```

### Comparing `jaxip-0.6.0/tests/test_md.py` & `jaxip-0.6.1/tests/test_structure.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,156 +1,182 @@
 import os
-from functools import partial
-from typing import Tuple
+from typing import Any, Dict, Tuple
 
-import jax
 import jax.numpy as jnp
 import pytest
-from ase import Atoms
 
 from jaxip.atoms.structure import Structure
-from jaxip.simulation.md import MDSimulator
-from jaxip.types import Array
-from jaxip.units import units
+from jaxip.types import dtype as _dtype
 
 os.environ["JAX_ENABLE_X64"] = "1"
 os.environ["JAX_PLATFORM_NAME"] = "cpu"
 
 
-def get_structure() -> Structure:
-    d = 6  # Angstrom
-    uc = Atoms("He", positions=[(d / 2, d / 2, d / 2)], cell=(d, d, d))
-    s = Structure.create_from_ase(uc.repeat((2, 2, 2)))
-    return s
-
-
-def get_potential():
-    @partial(jax.jit, static_argnums=0)
-    def _compute_pair_energy(obj, r: Array) -> Array:
-        term = obj.sigma / r
-        term6 = term**6
-        return 4.0 * obj.epsilon * term6 * (term6 - 1.0)
-
-    @partial(jax.jit, static_argnums=0)
-    def _compute_pair_force(obj, r: Array, R: Array) -> Array:
-        term = obj.sigma / r
-        term6 = term**6
-        force_factor = -24.0 * obj.epsilon / (r * r) * term6 * (2.0 * term6 - 1.0)
-        return jnp.expand_dims(force_factor, axis=-1) * R
-
-    class LJPotential:
-        def __init__(
-            self,
-            sigma: float,
-            epsilon: float,
-            r_cutoff: float,
-        ) -> None:
-            self.sigma = sigma
-            self.epsilon = epsilon
-            self.r_cutoff = r_cutoff
-
-        def __call__(self, structure: Structure) -> Array:
-            r, _ = structure.calculate_distance(atom_index=jnp.arange(structure.natoms))
-            mask = (0 < r) & (r < self.r_cutoff)
-            pair_energies = _compute_pair_energy(self, r)
-            return 0.5 * jnp.where(mask, pair_energies, 0.0).sum()  # type: ignore
-
-        def compute_force(self, structure: Structure) -> Array:
-            r, R = structure.calculate_distance(atom_index=jnp.arange(structure.natoms))
-            mask = (0 < r) & (r < self.r_cutoff)
-            pair_forces = jnp.where(
-                jnp.expand_dims(mask, axis=-1),
-                _compute_pair_force(self, r, R),
-                jnp.zeros_like(R),
-            )
-            return jnp.sum(pair_forces, axis=1)  # type: ignore
-
-    return LJPotential(
-        sigma=2.5238 * units.FROM_ANGSTROM,
-        epsilon=4.7093e-04 * units.FROM_ELECTRON_VOLT,
-        r_cutoff=6.3095 * units.FROM_ANGSTROM,
-    )
-
-
-class TestMDSimulator:
-    md = MDSimulator(
-        potential=get_potential(),
-        initial_structure=get_structure(),
-        time_step=0.5 * units.FROM_FEMTO_SECOND,
-        temperature=300,
+LJ_DATA: Dict[str, Any] = {
+    "position": [[0.0, 0.0, 0.0], [0.583123772, 0.583123772, 0.583123772]],
+    "element": ["Ne", "Ne"],
+    "charge": [0.0, 0.0],
+    "energy": [0.0, 0.0],
+    "force": [
+        [-11.4260918, -11.4260918, -11.4260918],
+        [11.4260918, 11.4260918, 11.4260918],
+    ],
+    "total_energy": [-0.21838404],
+    "comment": ["r = 1.01000000E+00, E = -2.18384040E-01, dEdr = -1.97905715E+01"],
+    "total_charge": [],
+    "lattice": [],
+    "atom_type": [1, 1],
+    "mass": [36785.88642640456] * 2,
+}
+
+H2O_DATA: Dict[str, Any] = {
+    "lattice": [
+        [11.8086403654, 0.0, 0.0],
+        [0.0, 11.8086403654, 0.0],
+        [0.0, 0.0, 11.8086403654],
+    ],
+    "position": [
+        [0.2958498542, -0.8444146738, 1.9618569793],
+        [1.7226932399, -1.8170359274, 0.5237867306],
+        [1.2660050151, -4.3958431356, 0.822408813],
+        [2.5830855482, 6.6971705174, 2.042321518],
+        [6.3733092527, 4.0651032678, 1.6571254123],
+        [4.5893132971, 4.2984466507, 3.33215409],
+        [-2.2136818837, 1.3673642557, 2.7768013741],
+        [-1.9466635812, -0.3397746484, 3.3828743394],
+        [-0.4559776878, 0.1681476423, -5.430449296],
+        [-1.2831542798, 4.5473991714, -2.294184217],
+        [-2.3516507887, 0.9376745482, -4.0756290424],
+        [-1.7819663898, 4.1957022409, -4.0621741923],
+    ],
+    "element": ["O", "H", "H", "O", "H", "H", "O", "H", "H", "O", "H", "H"],
+    "charge": [
+        0.423192,
+        -0.243872,
+        -0.313417,
+        0.439248,
+        -0.136408,
+        -0.154832,
+        0.418857,
+        -0.401243,
+        -0.0766178,
+        0.411994,
+        -0.0691934,
+        -0.297707,
+    ],
+    "energy": [
+        0.0,
+        0.0,
+        0.0,
+        0.0,
+        0.0,
+        0.0,
+        0.0,
+        0.0,
+        0.0,
+        0.0,
+        0.0,
+        0.0,
+    ],
+    "force": [
+        [-0.4727795521, -0.0084561951, 0.0460983059],
+        [0.1920381912, 0.0587784661, 0.6142110612],
+        [-0.8869675228, -0.7832124482, -0.7448845423],
+        [0.7405673293, 0.4095246028, 0.1627052569],
+        [-0.7272286968, 0.2123232582, 0.5568660265],
+        [0.6038769757, -0.0797700393, -0.5249089268],
+        [-0.2617806281, -0.2369410958, 0.1869405738],
+        [1.2121859011, 0.4399940142, -0.0045549514],
+        [-0.1108903386, -0.3317914324, -0.6560763592],
+        [-0.1172658121, -0.1885000212, -0.5958629059],
+        [-0.1934543148, 0.5415107499, 0.4505828542],
+        [0.0216973013, -0.0334599566, 0.508882732],
+    ],
+    "total_energy": [-32.1390027258],
+    "total_charge": [8.0e-07],
+    "atom_type": [2, 1, 1, 2, 1, 1, 2, 1, 1, 2, 1, 1],
+    "mass": [29164.39033379815, 1837.4714329938454, 1837.4714329938454] * 4,
+}
+
+
+class TestStructure:
+    lj: Structure = Structure.create_from_dict(
+        LJ_DATA, dtype=jnp.float32  # type: ignore
+    )  # type: ignore
+    h2o: Structure = Structure.create_from_dict(H2O_DATA, r_cutoff=11.0)
+    atom_attributes: Tuple[str, ...] = tuple(
+        ["position", "force", "energy", "total_energy", "charge", "total_charge"]
     )
 
     @pytest.mark.parametrize(
-        "md, expected",
+        "structure, expected",
         [
             (
-                md,
-                (
-                    0.5 * units.FROM_FEMTO_SECOND,
-                    262.15531167,
-                    5.70328776e-07,
-                    0.00995778,
-                    jnp.asarray([11.33835602, 11.33835602, 11.33835602]),
+                lj,
+                tuple(
+                    jnp.asarray(LJ_DATA[attr])
+                    for attr in Structure._get_atom_attributes()
                 ),
             ),
-        ],
-    )
-    def test_general_attributes(
-        self,
-        md: MDSimulator,
-        expected: Tuple,
-    ) -> None:
-        assert md.step == 0
-        assert jnp.allclose(md.elapsed_time, 0.0)
-        assert jnp.allclose(md.time_step, expected[0])
-        assert jnp.allclose(md.get_com_velocity(), jnp.zeros(3))
-        assert jnp.allclose(md.temperature, expected[1])
-        assert jnp.allclose(md.get_pressure(), expected[2])
-        assert jnp.allclose(md.get_total_energy(), expected[3])
-        assert jnp.allclose(md.get_com_position(), expected[4])
-
-    @pytest.mark.parametrize(
-        "md, structure",
-        [
             (
-                md,
-                get_structure(),
+                h2o,
+                tuple(
+                    jnp.asarray(H2O_DATA[attr])
+                    for attr in Structure._get_atom_attributes()
+                ),
             ),
         ],
     )
-    def test_structure_attributes(
+    def test_atom_attributes(
         self,
-        md: MDSimulator,
         structure: Structure,
+        expected: Tuple,
     ) -> None:
-        assert jnp.allclose(md.position, structure.position)
-        assert jnp.allclose(md.mass, structure.mass)
+        for i, attr in enumerate(Structure._get_atom_attributes()):
+            if attr == "position":
+                assert jnp.allclose(
+                    structure.position, structure.box.shift_inside_box(expected[i])
+                )
+            else:
+                assert jnp.allclose(getattr(structure, attr), expected[i])
 
     @pytest.mark.parametrize(
-        "md, expected",
+        "structure, expected",
         [
             (
-                md,
+                lj,
+                (
+                    2,
+                    ("Ne",),
+                    None,
+                    jnp.float32,
+                    None,
+                    jnp.asarray(LJ_DATA["mass"]),
+                ),
+            ),
+            (
+                h2o,
                 (
-                    0.5 * units.FROM_FEMTO_SECOND,
-                    260.89277174,
-                    5.68325481e-07,
-                    0.00992273,
-                    jnp.asarray([11.33835602, 11.33835602, 11.33835602]),
+                    12,
+                    ("H", "O"),
+                    11.0,
+                    _dtype.FLOATX,
+                    jnp.asarray(H2O_DATA["lattice"]),
+                    jnp.asarray(H2O_DATA["mass"]),
                 ),
             ),
         ],
     )
-    def test_md_step(
+    def test_general_attributes(
         self,
-        md: MDSimulator,
+        structure: Structure,
         expected: Tuple,
     ) -> None:
-        md.molecular_dynamics_step()
-        assert md.step == 1
-        assert jnp.allclose(md.elapsed_time, expected[0])
-        assert jnp.allclose(md.time_step, expected[0])
-        assert jnp.allclose(md.get_com_velocity(), jnp.zeros(3))
-        assert jnp.allclose(md.temperature, expected[1])
-        assert jnp.allclose(md.get_pressure(), expected[2])
-        assert jnp.allclose(md.get_total_energy(), expected[3])
-        assert jnp.allclose(md.get_com_position(), expected[4])
+        assert structure.natoms == expected[0]
+        assert structure.elements == expected[1]
+        assert structure.r_cutoff == expected[2]
+        assert structure.dtype == expected[3]
+        if structure.lattice is None:
+            assert structure.lattice is expected[4]
+        else:
+            assert jnp.allclose(structure.lattice, expected[4])
+        assert jnp.allclose(structure.mass, expected[5])
```

### Comparing `jaxip-0.6.0/tests/test_nn.py` & `jaxip-0.6.1/tests/test_nn.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 from jaxip.models.nn.initializer import UniformInitializer
 from jaxip.models.nn.network import NeuralNetworkModel
 from jaxip.types import dtype as _dtype
 
 
 class TestNeuralNetworkModel:
-
     nn_1: NeuralNetworkModel = NeuralNetworkModel(hidden_layers=((2, "tanh"),))
     nn_2: NeuralNetworkModel = NeuralNetworkModel(
         hidden_layers=((4, "tanh"), (8, "identity")),
         param_dtype=jnp.float64,  # type: ignore
     )
     nn_3: NeuralNetworkModel = NeuralNetworkModel(
         hidden_layers=((8, "tanh"), (16, "tanh")),
```

### Comparing `jaxip-0.6.0/tests/test_nnp.py` & `jaxip-0.6.1/tests/test_nnp.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 os.environ["JAX_PLATFORM_NAME"] = "cpu"
 
 import jax.numpy as jnp
 import pytest
 
 from jaxip.datasets import RunnerDataset
 from jaxip.potentials import NeuralNetworkPotential
-from jaxip.potentials.nnp.settings import (
-    NeuralNetworkPotentialSettings as PotentialSettings,
-)
+from jaxip.potentials.nnp.settings import \
+    NeuralNetworkPotentialSettings as PotentialSettings
 
 dataset_file = Path("tests", "h2o.data")
 potential_file = Path("tests", "h2o.json")
 
 
 class TestNeuralNetworkPotential:
     dataset = RunnerDataset(dataset_file)
```

### Comparing `jaxip-0.6.0/tests/test_runner.py` & `jaxip-0.6.1/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/tests/test_scaler.py` & `jaxip-0.6.1/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/tests/weights.001.pkl` & `jaxip-0.6.1/tests/weights.001.pkl`

 * *Files identical despite different names*

### Comparing `jaxip-0.6.0/tests/weights.008.pkl` & `jaxip-0.6.1/tests/weights.008.pkl`

 * *Files identical despite different names*

