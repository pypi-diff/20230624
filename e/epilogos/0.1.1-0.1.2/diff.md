# Comparing `tmp/epilogos-0.1.1.tar.gz` & `tmp/epilogos-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/epilogos-0.1.1.tar", last modified: Tue Jul 13 21:56:23 2021, max compression
+gzip compressed data, was "epilogos-0.1.2.tar", last modified: Fri Jun 23 23:21:10 2023, max compression
```

## Comparing `epilogos-0.1.1.tar` & `epilogos-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxr-xr-x   0 jquon      (965) stamlab    (506)        0 2021-07-13 21:56:23.000000 epilogos-0.1.1/
--rw-r--r--   0 jquon      (965) stamlab    (506)      106 2021-07-13 21:53:43.000000 epilogos-0.1.1/CHANGES.txt
--rw-r--r--   0 jquon      (965) stamlab    (506)       99 2021-05-25 21:04:03.000000 epilogos-0.1.1/MANIFEST.in
--rw-r--r--   0 jquon      (965) stamlab    (506)     4428 2021-07-13 21:56:23.000000 epilogos-0.1.1/PKG-INFO
--rw-r--r--   0 jquon      (965) stamlab    (506)     3452 2021-06-25 07:41:38.000000 epilogos-0.1.1/README.txt
-drwxr-xr-x   0 jquon      (965) stamlab    (506)        0 2021-07-13 21:56:22.000000 epilogos-0.1.1/bin/
--rwxr-xr-x   0 jquon      (965) stamlab    (506)     1680 2021-06-24 18:48:59.000000 epilogos-0.1.1/bin/download_example_data.sh
--rwxr-xr-x   0 jquon      (965) stamlab    (506)     2182 2021-06-24 18:48:59.000000 epilogos-0.1.1/bin/preprocess_data_ChromHMM.sh
-drwxr-xr-x   0 jquon      (965) stamlab    (506)        0 2021-07-13 21:56:23.000000 epilogos-0.1.1/epilogos/
--rw-r--r--   0 jquon      (965) stamlab    (506)       22 2021-07-13 21:54:31.000000 epilogos-0.1.1/epilogos/__init__.py
--rw-r--r--   0 jquon      (965) stamlab    (506)    10180 2021-06-02 21:02:12.000000 epilogos-0.1.1/epilogos/expected.py
--rw-r--r--   0 jquon      (965) stamlab    (506)     1606 2021-06-02 03:51:30.000000 epilogos-0.1.1/epilogos/expectedCombination.py
--rw-r--r--   0 jquon      (965) stamlab    (506)     6406 2021-06-02 21:02:12.000000 epilogos-0.1.1/epilogos/greatestHits.py
--rw-r--r--   0 jquon      (965) stamlab    (506)     7556 2021-06-02 21:02:12.000000 epilogos-0.1.1/epilogos/helpers.py
--rw-r--r--   0 jquon      (965) stamlab    (506)    47630 2021-06-24 23:55:37.000000 epilogos-0.1.1/epilogos/pairwiseVisual.py
--rw-r--r--   0 jquon      (965) stamlab    (506)    32686 2021-07-13 08:13:03.000000 epilogos-0.1.1/epilogos/run.py
--rw-r--r--   0 jquon      (965) stamlab    (506)    27073 2021-06-02 21:02:12.000000 epilogos-0.1.1/epilogos/scores.py
--rw-r--r--   0 jquon      (965) stamlab    (506)     6612 2021-05-18 21:13:16.000000 epilogos-0.1.1/epilogos/test.py
-drwxr-xr-x   0 jquon      (965) stamlab    (506)        0 2021-07-13 21:56:23.000000 epilogos-0.1.1/epilogos.egg-info/
--rw-r--r--   0 jquon      (965) stamlab    (506)     4428 2021-07-13 21:56:20.000000 epilogos-0.1.1/epilogos.egg-info/PKG-INFO
--rw-r--r--   0 jquon      (965) stamlab    (506)      513 2021-07-13 21:56:20.000000 epilogos-0.1.1/epilogos.egg-info/SOURCES.txt
--rw-r--r--   0 jquon      (965) stamlab    (506)        1 2021-07-13 21:56:20.000000 epilogos-0.1.1/epilogos.egg-info/dependency_links.txt
--rw-r--r--   0 jquon      (965) stamlab    (506)       48 2021-07-13 21:56:20.000000 epilogos-0.1.1/epilogos.egg-info/entry_points.txt
--rw-r--r--   0 jquon      (965) stamlab    (506)      181 2021-07-13 21:56:20.000000 epilogos-0.1.1/epilogos.egg-info/requires.txt
--rw-r--r--   0 jquon      (965) stamlab    (506)        9 2021-07-13 21:56:20.000000 epilogos-0.1.1/epilogos.egg-info/top_level.txt
--rw-r--r--   0 jquon      (965) stamlab    (506)      180 2021-06-11 21:43:03.000000 epilogos-0.1.1/requirements.txt
--rw-r--r--   0 jquon      (965) stamlab    (506)       38 2021-07-13 21:56:23.000000 epilogos-0.1.1/setup.cfg
--rw-r--r--   0 jquon      (965) stamlab    (506)     1104 2021-06-25 07:35:50.000000 epilogos-0.1.1/setup.py
+drwxr-xr-x   0 jquon      (965) stamlab    (506)        0 2023-06-23 23:21:10.654187 epilogos-0.1.2/
+-rw-r--r--   0 jquon      (965) stamlab    (506)     2415 2023-06-23 23:16:46.000000 epilogos-0.1.2/CHANGES.txt
+-rw-r--r--   0 jquon      (965) stamlab    (506)    35149 2021-03-29 17:37:54.000000 epilogos-0.1.2/LICENSE
+-rw-r--r--   0 jquon      (965) stamlab    (506)       99 2021-05-25 21:04:03.000000 epilogos-0.1.2/MANIFEST.in
+-rw-r--r--   0 jquon      (965) stamlab    (506)     3859 2023-06-23 23:21:10.653192 epilogos-0.1.2/PKG-INFO
+-rw-r--r--   0 jquon      (965) stamlab    (506)     3492 2023-06-21 21:41:38.000000 epilogos-0.1.2/README.txt
+drwxr-xr-x   0 jquon      (965) stamlab    (506)        0 2023-06-23 23:21:10.287193 epilogos-0.1.2/bin/
+-rwxr-xr-x   0 jquon      (965) stamlab    (506)     5728 2022-11-07 22:29:56.000000 epilogos-0.1.2/bin/download_example_data.sh
+-rwxr-xr-x   0 jquon      (965) stamlab    (506)     2182 2021-06-24 18:48:59.000000 epilogos-0.1.2/bin/preprocess_data_ChromHMM.sh
+drwxr-xr-x   0 jquon      (965) stamlab    (506)        0 2023-06-23 23:21:10.603190 epilogos-0.1.2/epilogos/
+-rw-r--r--   0 jquon      (965) stamlab    (506)       22 2023-06-23 23:17:42.000000 epilogos-0.1.2/epilogos/__init__.py
+-rw-r--r--   0 jquon      (965) stamlab    (506)    10493 2023-01-07 09:02:19.000000 epilogos-0.1.2/epilogos/expected.py
+-rw-r--r--   0 jquon      (965) stamlab    (506)     1724 2023-01-07 09:02:19.000000 epilogos-0.1.2/epilogos/expectedCombination.py
+-rw-r--r--   0 jquon      (965) stamlab    (506)    17967 2023-06-21 21:41:38.000000 epilogos-0.1.2/epilogos/filter_regions.py
+-rw-r--r--   0 jquon      (965) stamlab    (506)    12725 2023-06-21 21:41:38.000000 epilogos-0.1.2/epilogos/helpers.py
+-rw-r--r--   0 jquon      (965) stamlab    (506)    20974 2023-01-07 09:02:19.000000 epilogos-0.1.2/epilogos/plotRegion.py
+-rw-r--r--   0 jquon      (965) stamlab    (506)    61660 2023-01-27 23:00:38.000000 epilogos-0.1.2/epilogos/roiAndVisualPairwise.py
+-rw-r--r--   0 jquon      (965) stamlab    (506)     6522 2023-01-07 09:02:19.000000 epilogos-0.1.2/epilogos/roiSingle.py
+-rw-r--r--   0 jquon      (965) stamlab    (506)    34431 2023-06-22 20:35:30.000000 epilogos-0.1.2/epilogos/run.py
+-rw-r--r--   0 jquon      (965) stamlab    (506)    28068 2023-01-07 09:02:19.000000 epilogos-0.1.2/epilogos/scores.py
+-rw-r--r--   0 jquon      (965) stamlab    (506)     8665 2023-01-27 20:48:03.000000 epilogos-0.1.2/epilogos/similaritySearch_calc.py
+-rw-r--r--   0 jquon      (965) stamlab    (506)     7670 2023-01-27 20:48:03.000000 epilogos-0.1.2/epilogos/similaritySearch_max_mean.py
+-rw-r--r--   0 jquon      (965) stamlab    (506)    23078 2023-01-27 20:48:03.000000 epilogos-0.1.2/epilogos/similaritySearch_run.py
+-rw-r--r--   0 jquon      (965) stamlab    (506)     8435 2023-06-13 21:03:58.000000 epilogos-0.1.2/epilogos/similaritySearch_write.py
+drwxr-xr-x   0 jquon      (965) stamlab    (506)        0 2023-06-23 23:21:10.649195 epilogos-0.1.2/epilogos.egg-info/
+-rw-r--r--   0 jquon      (965) stamlab    (506)     3859 2023-06-23 23:21:08.000000 epilogos-0.1.2/epilogos.egg-info/PKG-INFO
+-rw-r--r--   0 jquon      (965) stamlab    (506)      697 2023-06-23 23:21:08.000000 epilogos-0.1.2/epilogos.egg-info/SOURCES.txt
+-rw-r--r--   0 jquon      (965) stamlab    (506)        1 2023-06-23 23:21:08.000000 epilogos-0.1.2/epilogos.egg-info/dependency_links.txt
+-rw-r--r--   0 jquon      (965) stamlab    (506)      132 2023-06-23 23:21:08.000000 epilogos-0.1.2/epilogos.egg-info/entry_points.txt
+-rw-r--r--   0 jquon      (965) stamlab    (506)      172 2023-06-23 23:21:08.000000 epilogos-0.1.2/epilogos.egg-info/requires.txt
+-rw-r--r--   0 jquon      (965) stamlab    (506)        9 2023-06-23 23:21:08.000000 epilogos-0.1.2/epilogos.egg-info/top_level.txt
+-rw-r--r--   0 jquon      (965) stamlab    (506)      172 2023-06-21 21:41:38.000000 epilogos-0.1.2/requirements.txt
+-rw-r--r--   0 jquon      (965) stamlab    (506)       38 2023-06-23 23:21:10.654197 epilogos-0.1.2/setup.cfg
+-rw-r--r--   0 jquon      (965) stamlab    (506)     1217 2022-12-24 00:20:04.000000 epilogos-0.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `epilogos-0.1.1/PKG-INFO` & `epilogos-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,87 @@
 Metadata-Version: 2.1
 Name: epilogos
-Version: 0.1.1
+Version: 0.1.2
 Summary: Information-theoretic navigation of multi-tissue functional genomic annotations
 Home-page: https://github.com/meuleman/epilogos
 Author: Wouter Meuleman, Jacob Quon, Alex Reynolds, Eric Rynes
 Author-email: wouter@meuleman.org
 License: LICENSE.txt
-Description: .. image:: https://raw.githubusercontent.com/meuleman/epilogos/main/data/logo.png
-          :width: 840
-          :alt: Epilogos
-        
-        ------
-        
-        
-        Information-theoretic navigation of multi-tissue functional genomic annotations
-        ===============================================================================
-        
-        Epilogos is an approach for analyzing, visualizing, and navigating multi-biosample functional genomic annotations, with an emphasis on chromatin state maps generated with e.g. ChromHMM or Segway.
-        
-        The software provided in this repository implements the methods underlying Epilogos using Python 3.7. We provide a proof-of-principle dataset based on chromatin state calls from the EpiMap dataset (`Boix et al., Nature 2021 <https://www.nature.com/articles/s41586-020-03145-z>`_).
-        
-        Created by: Wouter Meuleman, Jacob Quon, Alex Reynolds, and Eric Rynes
-        
-        ------
-        
-        
-        Installation
-        ============
-        
-        Although not required, it is good practice to create a virtual environment in which
-        specific versions of Python and its libraries are installed.
-        This can be done using ``conda``, for instance as such:
-        
-        .. code-block:: bash
-        
-            $ conda init bash  ## only needed upon first use of conda. Restart shell after this.
-            $ conda create -n epilogos python=3.8
-            $ conda activate epilogos
-        
-        To install Epilogos simply run the following command
-        
-        .. code-block:: bash
-        
-            $ pip install epilogos
-        
-        Alternatively, install Epilogos directly from the Git repositority using
-        
-        .. code-block:: bash
-        
-            $ pip install git+https://github.com/meuleman/epilogos
-        
-        
-        Prerequisites
-        =============
-        
-        To compute epilogos, you will need to have the following python libraries installed: `cython <https://cython.org/>`_, `pyranges <https://github.com/biocore-ntnu/pyranges>`_, `statsmodels <https://www.statsmodels.org/stable/index.html>`_, `click <https://click.palletsprojects.com/en/7.x/>`_, `numpy <https://numpy.org/>`_, `scipy <https://www.scipy.org/>`_, `matplotlib <https://matplotlib.org/stable/index.html>`_, and `pandas <https://pandas.pydata.org/>`_. These can be installed with one of the following commands
-        
-        .. code-block:: bash
-        
-            $ pip install 'cython>=0.29.23,<1.0.0'; pip install 'click>=7.1.2,<8.0.0' 'numpy>=1.19.2,<2.0.0' 'pandas>=1.1.3,<2.0.0' 'pyranges>=0.0.97,<1.0.0' 'scipy>=1.5.2,<2.0.0' 'matplotlib>=3.3.2,<4.0.0' 'statsmodels>=0.12.0,<1.0.0'
-        
-        or while in the epilogos directory (we use cat and xargs to ensure installation order as pyranges is dependent on cython)
-        
-        .. code-block:: bash
-        
-            $ cat requirements.txt | xargs -n 1 -L 1 pip install
-        
-        
-        Additionally, it is recommended that python is updated to version 3.7 or later. In earlier python versions, ``src/scores.py`` may raise an OSError 16. It is worth noting that in our testing this error has not affected the results.
-        
-        
-        Running Epilogos
-        ================
-        
-        To be presented with basic documentation of arguments needed to run epilogos, simply run the command ``epilogos --help`` or ``python -m epilogos --help`` (More in-depth explanation is given on the `github README <https://github.com/meuleman/epilogos)>`_).
-        
-        By default, Epilogos assumes access to a computational cluster managed by `SLURM <https://slurm.schedmd.com/>`_.
-        A version of epilogos has been created for those without access to a SLURM cluster and can be run by using the ``-l`` flag to your command (e.g. ``epilogos -l``).
-        
-        --------------
-        
-        For a more extensive set of documentation, please refer to `our github <https://github.com/meuleman/epilogos>`_.
-        
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+.. image:: https://raw.githubusercontent.com/meuleman/epilogos/main/data/logo.png
+  :width: 840
+  :alt: Epilogos
+
+------
+
+
+Information-theoretic navigation of multi-tissue functional genomic annotations
+===============================================================================
+
+Epilogos is an approach for analyzing, visualizing, and navigating multi-biosample functional genomic annotations, with an emphasis on chromatin state maps generated with e.g. ChromHMM or Segway.
+
+The software provided in this repository implements the methods underlying Epilogos using Python 3.9. We provide a proof-of-principle dataset based on chromatin state calls from the EpiMap dataset (`Boix et al., Nature 2021 <https://www.nature.com/articles/s41586-020-03145-z>`_).
+
+Created by: Wouter Meuleman, Jacob Quon, Alex Reynolds, and Eric Rynes
+
+------
+
+
+Installation
+============
+
+Although not required, it is good practice to create a virtual environment in which
+specific versions of Python and its libraries are installed.
+This can be done using ``conda``, for instance as such:
+
+.. code-block:: bash
+
+    $ conda init bash  ## only needed upon first use of conda. Restart shell after this.
+    $ conda create -n epilogos python=3.9
+    $ conda activate epilogos
+
+To install Epilogos simply run the following two commands
+
+.. code-block:: bash
+
+    $ pip install epilogos
+
+Alternatively, install Epilogos directly from the Git repositority using
+
+.. code-block:: bash
+
+    $ pip install git+https://github.com/meuleman/epilogos
+
+
+Prerequisites
+=============
+
+To compute epilogos, you will need to have the following python libraries installed: `statsmodels <https://www.statsmodels.org/stable/index.html>`_, `click <https://click.palletsprojects.com/en/7.x/>`_, `numpy <https://numpy.org/>`_, `scipy <https://www.scipy.org/>`_, `matplotlib <https://matplotlib.org/stable/index.html>`_, `pandas <https://pandas.pydata.org/>`_, `pysam <https://pysam.readthedocs.io/en/latest/api.html>`_, `scikit-learn <https://scikit-learn.org/stable/>`_, `natsort <https://natsort.readthedocs.io/en/stable/>`_, `pyranges <https://pyranges.readthedocs.io/en/latest/autoapi/pyranges/index.html>`_, and `rich <https://rich.readthedocs.io/en/stable/index.html>`_.
+These can be installed with one of the following commands
+
+.. code-block:: bash
+
+    $ pip install 'click==8.1.3' 'numpy==1.23.4' 'pandas==1.5.1' 'scipy==1.9.3' 'matplotlib==3.6.1' 'statsmodels==0.13.2' 'scikit-learn==1.1.3' 'pysam==0.19.1' 'natsort==8.2.0' 'pyranges==0.0.117' 'rich==12.6.0'
+
+or while in the epilogos directory
+
+.. code-block:: bash
+
+    $ pip install -r requirements.txt
+
+
+Additionally, it is recommended that python is updated to version 3.9 or later. We cannot guarantee the validity of results generated by earlier verions of python.
+
+
+Running Epilogos
+================
+
+To be presented with basic documentation of arguments needed to run epilogos, simply run the command ``epilogos --help`` or ``python -m epilogos --help`` (More in-depth explanation is given on the `github README <https://github.com/meuleman/epilogos)>`_).
+
+By default, Epilogos assumes access to a computational cluster managed by `SLURM <https://slurm.schedmd.com/>`_.
+A version of epilogos has been created for those without access to a SLURM cluster and can be run by using the ``-l`` flag to your command (e.g. ``epilogos -l``).
+
+--------------
+
+For a more extensive set of documentation, please refer to `our github <https://github.com/meuleman/epilogos>`_.
```

### Comparing `epilogos-0.1.1/README.txt` & `epilogos-0.1.2/README.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 Information-theoretic navigation of multi-tissue functional genomic annotations
 ===============================================================================
 
 Epilogos is an approach for analyzing, visualizing, and navigating multi-biosample functional genomic annotations, with an emphasis on chromatin state maps generated with e.g. ChromHMM or Segway.
 
-The software provided in this repository implements the methods underlying Epilogos using Python 3.7. We provide a proof-of-principle dataset based on chromatin state calls from the EpiMap dataset (`Boix et al., Nature 2021 <https://www.nature.com/articles/s41586-020-03145-z>`_).
+The software provided in this repository implements the methods underlying Epilogos using Python 3.9. We provide a proof-of-principle dataset based on chromatin state calls from the EpiMap dataset (`Boix et al., Nature 2021 <https://www.nature.com/articles/s41586-020-03145-z>`_).
 
 Created by: Wouter Meuleman, Jacob Quon, Alex Reynolds, and Eric Rynes
 
 ------
 
 
 Installation
@@ -23,18 +23,18 @@
 Although not required, it is good practice to create a virtual environment in which
 specific versions of Python and its libraries are installed.
 This can be done using ``conda``, for instance as such:
 
 .. code-block:: bash
 
     $ conda init bash  ## only needed upon first use of conda. Restart shell after this.
-    $ conda create -n epilogos python=3.8
+    $ conda create -n epilogos python=3.9
     $ conda activate epilogos
 
-To install Epilogos simply run the following command
+To install Epilogos simply run the following two commands
 
 .. code-block:: bash
 
     $ pip install epilogos
 
 Alternatively, install Epilogos directly from the Git repositority using
 
@@ -42,28 +42,29 @@
 
     $ pip install git+https://github.com/meuleman/epilogos
 
 
 Prerequisites
 =============
 
-To compute epilogos, you will need to have the following python libraries installed: `cython <https://cython.org/>`_, `pyranges <https://github.com/biocore-ntnu/pyranges>`_, `statsmodels <https://www.statsmodels.org/stable/index.html>`_, `click <https://click.palletsprojects.com/en/7.x/>`_, `numpy <https://numpy.org/>`_, `scipy <https://www.scipy.org/>`_, `matplotlib <https://matplotlib.org/stable/index.html>`_, and `pandas <https://pandas.pydata.org/>`_. These can be installed with one of the following commands
+To compute epilogos, you will need to have the following python libraries installed: `statsmodels <https://www.statsmodels.org/stable/index.html>`_, `click <https://click.palletsprojects.com/en/7.x/>`_, `numpy <https://numpy.org/>`_, `scipy <https://www.scipy.org/>`_, `matplotlib <https://matplotlib.org/stable/index.html>`_, `pandas <https://pandas.pydata.org/>`_, `pysam <https://pysam.readthedocs.io/en/latest/api.html>`_, `scikit-learn <https://scikit-learn.org/stable/>`_, `natsort <https://natsort.readthedocs.io/en/stable/>`_, `pyranges <https://pyranges.readthedocs.io/en/latest/autoapi/pyranges/index.html>`_, and `rich <https://rich.readthedocs.io/en/stable/index.html>`_.
+These can be installed with one of the following commands
 
 .. code-block:: bash
 
-    $ pip install 'cython>=0.29.23,<1.0.0'; pip install 'click>=7.1.2,<8.0.0' 'numpy>=1.19.2,<2.0.0' 'pandas>=1.1.3,<2.0.0' 'pyranges>=0.0.97,<1.0.0' 'scipy>=1.5.2,<2.0.0' 'matplotlib>=3.3.2,<4.0.0' 'statsmodels>=0.12.0,<1.0.0'
+    $ pip install 'click==8.1.3' 'numpy==1.23.4' 'pandas==1.5.1' 'scipy==1.9.3' 'matplotlib==3.6.1' 'statsmodels==0.13.2' 'scikit-learn==1.1.3' 'pysam==0.19.1' 'natsort==8.2.0' 'pyranges==0.0.117' 'rich==12.6.0'
 
-or while in the epilogos directory (we use cat and xargs to ensure installation order as pyranges is dependent on cython)
+or while in the epilogos directory
 
 .. code-block:: bash
 
-    $ cat requirements.txt | xargs -n 1 -L 1 pip install
+    $ pip install -r requirements.txt
 
 
-Additionally, it is recommended that python is updated to version 3.7 or later. In earlier python versions, ``src/scores.py`` may raise an OSError 16. It is worth noting that in our testing this error has not affected the results.
+Additionally, it is recommended that python is updated to version 3.9 or later. We cannot guarantee the validity of results generated by earlier verions of python.
 
 
 Running Epilogos
 ================
 
 To be presented with basic documentation of arguments needed to run epilogos, simply run the command ``epilogos --help`` or ``python -m epilogos --help`` (More in-depth explanation is given on the `github README <https://github.com/meuleman/epilogos)>`_).
```

### Comparing `epilogos-0.1.1/bin/preprocess_data_ChromHMM.sh` & `epilogos-0.1.2/bin/preprocess_data_ChromHMM.sh`

 * *Files identical despite different names*

### Comparing `epilogos-0.1.1/epilogos/expected.py` & `epilogos-0.1.2/epilogos/expected.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import numpy as np
 from sys import argv
 from pathlib import Path
 from time import time
 from multiprocessing import cpu_count, Pool
 from itertools import repeat, permutations
 from contextlib import closing
-from epilogos.helpers import strToBool, splitRows, readStates
+from epilogos.helpers import strToBool, countRows, splitRows, readStates
 
 
 def main(file1, file2, numStates, saliency, outputDir, fileTag, numProcesses, verbose):
     """
     Wrapper function which prepares inputs for the expected frequency calculation
 
     Input:
-    file1 -- The path of the only (single epilogos) or first (paired epilogos) file to read states from
-    file2 -- The path of the second file to read states from (paired epilogos)
-    numStates -- The number of states in the state model
-    saliency -- The saliency metric being used in the epilogos run
-    outputDir -- The path of the output directory
-    fileTag -- A string which helps ensure outputed files are named similarly within an epilogos run
+    file1        -- The path of the only (single epilogos) or first (paired epilogos) file to read states from
+    file2        -- The path of the second file to read states from (paired epilogos)
+    numStates    -- The number of states in the state model
+    saliency     -- The saliency metric being used in the epilogos run
+    outputDir    -- The path of the output directory
+    fileTag      -- A string which helps ensure outputed files are named similarly within an epilogos run
     numProcesses -- The number of cores to run on
-    verbose -- Boolean which if True, causes much more detailed prints
+    verbose      -- Boolean which if True, causes much more detailed prints
     """
     if verbose: tTotal = time()
 
     file1Path = Path(file1)
     file2Path = Path(file2)
     outputDirPath = Path(outputDir)
 
@@ -33,38 +33,41 @@
     if not verbose: print("    {}\t".format(filename), end="", flush=True)
 
     # If user doesn't want to choose number of cores, use as many as available
     if numProcesses == 0:
         numProcesses = cpu_count()
 
     # Determine which rows to assign to each core
-    rowList = splitRows(file1Path, numProcesses)
+    rowList = splitRows(countRows(file1Path), numProcesses)
 
-    calculateExpected(saliency, file1Path, file2Path, rowList, numStates, outputDirPath, fileTag, filename, numProcesses,
-                      verbose)
+    calculateExpected(saliency, file1Path, file2Path, rowList, numStates, outputDirPath, fileTag, filename,
+                      numProcesses, verbose)
 
     print("Total Time:", time() - tTotal, flush=True) if verbose else print("\t[Done]", flush=True)
 
 
-def calculateExpected(saliency, file1Path, file2Path, rowList, numStates, outputDirPath, fileTag, filename, numProcesses,
-                      verbose):
+def calculateExpected(saliency, file1Path, file2Path, rowList, numStates, outputDirPath, fileTag, filename,
+                      numProcesses, verbose):
     """
     Function responsible for deploying the processes used to calculate the expected frequencies
 
     Input:
-    saliency -- The saliency metric being used in the epilogos run
-    file1Path -- The path of the only (single epilogos) or first (paired epilogos) file to read states from
-    file2Path -- The path of the second file to read states from (paired epilogos)
-    rowList -- A list of tuples which contain the first and last rows for each core to use
-    numStates -- The number of states in the state model
+    saliency      -- The saliency metric being used in the epilogos run
+    file1Path     -- The path of the only (single epilogos) or first (paired epilogos) file to read states from
+    file2Path     -- The path of the second file to read states from (paired epilogos)
+    rowList       -- A list of tuples which contain the first and last rows for each core to use
+    numStates     -- The number of states in the state model
     outputDirPath -- The path of the output directory
-    fileTag -- A string which helps ensure outputed files are named similarly within an epilogos run
-    filename -- The name of the file for which we are calculating the expected frequencies
-    numProcesses -- The number of cores to run on
-    verbose -- Boolean which if True, causes much more detailed prints
+    fileTag       -- A string which helps ensure outputed files are named similarly within an epilogos run
+    filename      -- The name of the file for which we are calculating the expected frequencies
+    numProcesses  -- The number of cores to run on
+    verbose       -- Boolean which if True, causes much more detailed prints
+
+    Output:
+    A .npy array containing the expected frequencies of the input file
     """
     if verbose: print("\nNumber of Processes:", numProcesses, flush=True)
 
     # Start the processes
     with closing(Pool(numProcesses)) as pool:
         if saliency == 1:
             results = pool.starmap(s1Calc, zip(repeat(file1Path), repeat(file2Path), rowList, repeat(numStates),
@@ -85,26 +88,26 @@
 
 
 def s1Calc(file1Path, file2Path, rowsToCalc, numStates, verbose):
     """
     Function responsible for expected frequency calculation over a set of rows for a saliency metric of 1
 
     Input:
-    file1Path -- The path of the only (single epilogos) or first (paired epilogos) file to read states from
-    file2Path -- The path of the second file to read states from (paired epilogos)
+    file1Path  -- The path of the only (single epilogos) or first (paired epilogos) file to read states from
+    file2Path  -- The path of the second file to read states from (paired epilogos)
     rowsToCalc -- The rows to count expected frequencies from the files
-    numStates -- The number of states in the state model
-    verbose -- Boolean which if True, causes much more detailed prints
+    numStates  -- The number of states in the state model
+    verbose    -- Boolean which if True, causes much more detailed prints
 
     Output:
     A numpy array containing the counts of each state within the specified rows of the file
     """
     dataArr = readStates(file1Path=file1Path, file2Path=file2Path, rowsToCalc=rowsToCalc, verbose=verbose)
 
-    expFreqArr = np.zeros(numStates, dtype=np.int32)
+    expFreqArr = np.zeros(numStates, dtype=np.int64)
 
     if verbose and rowsToCalc[0] == 0: print("Calculating expected frequencies...", flush=True); tExp = time()
 
     # Simply count all states across out our subset of data
     uniqueStates, stateCounts = np.unique(dataArr, return_counts=True)
     for i, state in enumerate(uniqueStates):
         expFreqArr[state] += stateCounts[i]
@@ -114,30 +117,31 @@
 
 
 def s2Calc(file1Path, file2Path, rowsToCalc, numStates, verbose):
     """
     Function responsible for expected frequency calculation over a set of rows for a saliency metric of 2
 
     Input:
-    file1Path -- The path of the only (single epilogos) or first (paired epilogos) file to read states from
-    file2Path -- The path of the second file to read states from (paired epilogos)
+    file1Path  -- The path of the only (single epilogos) or first (paired epilogos) file to read states from
+    file2Path  -- The path of the second file to read states from (paired epilogos)
     rowsToCalc -- The rows to count expected frequencies from the files
-    numStates -- The number of states in the state model
-    verbose -- Boolean which if True, causes much more detailed prints
+    numStates  -- The number of states in the state model
+    verbose    -- Boolean which if True, causes much more detailed prints
 
     Output:
     A numpy array containing the counts of each pair of states within the specified rows of the file
     """
     dataArr = readStates(file1Path=file1Path, file2Path=file2Path, rowsToCalc=rowsToCalc, verbose=verbose)
 
     multiprocessRows = dataArr.shape[0]
 
-    expFreqArr = np.zeros((numStates, numStates), dtype=np.int32)
+    expFreqArr = np.zeros((numStates, numStates), dtype=np.int64)
 
-    if verbose and rowsToCalc[0] == 0: print("Calculating expected frequencies...", flush=True); tExp = time(); percentDone = 0
+    if verbose and rowsToCalc[0] == 0:
+        print("Calculating expected frequencies...", flush=True); tExp = time(); percentDone = 0
     printCheckmarks = [int(multiprocessRows * float(i / 10)) for i in range(1, 10)]
 
     # SumOverRows: Within a row, how many ways can you choose x and y to be together (will normalize later)
     # Can choose x and y to be together n*m ways if n != m and n(n-1) ways if n == m
     # (where n and m are the number of times that x and y show up respectively)
     for row in range(multiprocessRows):
 
@@ -145,46 +149,47 @@
             print("    {}% Completed".format(percentDone), flush=True)
         if not verbose and rowsToCalc[0] == 0 and row in printCheckmarks: print(".", end="", flush=True)
 
         uniqueStates, stateCounts = np.unique(dataArr[row], return_counts=True)
         for i, state1 in enumerate(uniqueStates):
             for j, state2 in enumerate(uniqueStates):
                 if state1 == state2:
-                    expFreqArr[state1, state2] += stateCounts[i] * (stateCounts[i] - 1)
+                    expFreqArr[state1, state2] += stateCounts[i] * (stateCounts[j] - 1)
                 else:  # state1 > state2 or state1 < state2
                     expFreqArr[state1, state2] += stateCounts[i] * stateCounts[j]
 
     if verbose and rowsToCalc[0] == 0: print("    Time:", time() - tExp, flush=True)
 
     return expFreqArr
 
 
 def s3Calc(file1Path, rowsToCalc, numStates, verbose):
     """
-    Function responsible for expected frequency calculation over a set of rows for a saliency metric of 2
+    Function responsible for expected frequency calculation over a set of rows for a saliency metric of 3
 
     Input:
-    file1Path -- The path of the only file to read states from
+    file1Path  -- The path of the only file to read states from
     rowsToCalc -- The first and last rows to count expected frequencies from the file
-    numStates -- The number of states in the state model
-    verbose -- Boolean which if True, causes much more detailed prints
+    numStates  -- The number of states in the state model
+    verbose    -- Boolean which if True, causes much more detailed prints
 
     Output:
     A numpy array containing the counts of each grouping of states and epigenomes within the specified rows of the file
     """
     dataArr = readStates(file1Path=file1Path, rowsToCalc=rowsToCalc, verbose=verbose)
 
     multiprocessRows, numCols = dataArr.shape
 
     # Gives us everyway to combine the column numbers in numpy indexing form
     basePermutationArr = np.array(list(permutations(range(numCols), 2))).T
 
     expFreqArr = np.zeros((numCols, numCols, numStates, numStates), dtype=np.int32)
 
-    if verbose and rowsToCalc[0] == 0: print("Calculating expected frequencies...", flush=True); tExp = time(); percentDone = 0
+    if verbose and rowsToCalc[0] == 0:
+        print("Calculating expected frequencies...", flush=True); tExp = time(); percentDone = 0
     printCheckmarks = [int(multiprocessRows * float(i / 10)) for i in range(1, 10)]
 
     # We tally a one for all the state/column combinations we observe
     # (e.g. for state 18 in column 2 and state 15 in column 6 we would add one to index [5, 1, 17, 14])
     for row in range(multiprocessRows):
 
         if verbose and rowsToCalc[0] == 0 and row in printCheckmarks: percentDone += 10; \
@@ -200,20 +205,23 @@
 
 
 def storeExpArray(expFreqArr, outputDirPath, fileTag, filename):
     """
     Stores the expected frequency array of the file as a temporary .npy file
 
     Input:
-    expFreqArr -- Numpy array of the expected frequencies
+    expFreqArr    -- Numpy array of the expected frequencies
     outputDirPath -- The output directory for epilogos
-    fileTag -- A string which helps ensure outputed files are named similarly within an epilogos run
-    filename -- The name of the file for which we calculated the expected frequencies
+    fileTag       -- A string which helps ensure outputed files are named similarly within an epilogos run
+    filename      -- The name of the file for which we calculated the expected frequencies
+
+    Output:
+    A .npy array containing the expected frequencies of the input file
     """
     expFreqFilename = "temp_exp_freq_{}_{}.npy".format(fileTag, filename)
     expFreqPath = outputDirPath / expFreqFilename
 
     np.save(expFreqPath, expFreqArr, allow_pickle=False)
 
 
 if __name__ == "__main__":
-    main(argv[1], argv[2], int(argv[3]), int(argv[4]), argv[5], argv[6], int(argv[7]), strToBool(argv[8]))
+    main(argv[1], argv[2], int(argv[3]), int(argv[4]), argv[5], argv[6], int(argv[7]), strToBool(argv[8]))
```

### Comparing `epilogos-0.1.1/epilogos/expectedCombination.py` & `epilogos-0.1.2/epilogos/expectedCombination.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,20 @@
 
 def main(outputDirectory, storedExpInput, fileTag, verbose):
     """
     Combines all the temporary expected frequency numpy arrays into one expected frequency array
 
     Input:
     outputDirectory -- The output directory for epilogos
-    storedExpInput -- The path of the expected frequency array which is being created
-    fileTag -- A string which helps ensure outputed files are named similarly within an epilogos run
-    verbose -- Boolean which if True, causes much more detailed prints
+    storedExpInput  -- The path of the expected frequency array which is being created
+    fileTag         -- A string which helps ensure outputed files are named similarly within an epilogos run
+    verbose         -- Boolean which if True, causes much more detailed prints
+
+    Output:
+    A .npy file containing an array of the expected frequencies across all input files
     """
     if verbose: tTotal = time()
 
     outputDirPath = Path(outputDirectory)
     storedExpPath = Path(storedExpInput)
 
     # Loop over all the expected value arrays and add them up
@@ -40,8 +43,8 @@
 
     np.save(storedExpPath, expFreqArr, allow_pickle=False)
 
     print("Total Time:", time() - tTotal) if verbose else print("    [Done]")
 
 
 if __name__ == "__main__":
-    main(argv[1], argv[2], argv[3], strToBool(argv[4]))
+    main(argv[1], argv[2], argv[3], strToBool(argv[4]))
```

### Comparing `epilogos-0.1.1/epilogos/greatestHits.py` & `epilogos-0.1.2/epilogos/roiSingle.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 from sys import argv
 from pathlib import Path
 import numpy as np
 from time import time
 from os import remove
 import pandas as pd
-import pyranges as pr
-from epilogos.pairwiseVisual import mergeAdjacent, findSign
-from epilogos.helpers import strToBool, getStateNames
+from epilogos.helpers import maxMean, generateROIIndicesArr, orderChromosomes, strToBool, getStateNames, findSign
 
 
-def main(outputDir, stateInfo, fileTag, expFreqPath, verbose):
+def main(outputDir, stateInfo, fileTag, expFreqPath, roiWidth, verbose):
     """
     Finds the top scoring regions across all epilogos score files and puts them into a txt file
 
     Input:
-    outputDir -- The path of the output directory
-    stateInfo -- State model tab seperated information file
-    fileTag -- A string which helps ensure outputed files are named similarly within an epilogos run
+    outputDir   -- The path of the output directory
+    stateInfo   -- State model tab seperated information file
+    fileTag     -- A string which helps ensure outputed files are named similarly within an epilogos run
     expFreqPath -- The location of the stored expected frequency array
-    verbose -- Boolean which if True, causes much more detailed prints
+    roiWidth    -- Size of regions of interest in bins
+    verbose     -- Boolean which if True, causes much more detailed prints
     """
     outputDirPath = Path(outputDir)
 
     stateNameList = getStateNames(stateInfo)
 
     if verbose: print("\nReading in score files...", flush=True); tRead = time()
     else: print("    Reading in files\t", end="", flush=True)
-    locationArr, scoreArr, maxScoreArr = readInData(outputDirPath)
+    locationArr, scoreArr = readInData(outputDirPath)
     if verbose: print("    Time:", time() - tRead, flush=True)
     else: print("\t[Done]", flush=True)
 
-    if verbose: print("\nFinding greatest hits...", flush=True); tHits = time()
-    else: print("    Greatest hits txt\t", end="", flush=True)
-    greatestHitsPath = outputDirPath / "greatestHits_{}.txt".format(fileTag)
-    createTopScoresTxt(greatestHitsPath, locationArr, scoreArr, maxScoreArr, stateNameList)
-    if verbose: print("    Time:", time() - tHits, flush=True)
+    if verbose: print("\nFinding regions of interest...", flush=True); tRoi = time()
+    else: print("    Regions of interest txt\t", end="", flush=True)
+    roiPath = outputDirPath / "regionsOfInterest_{}.txt".format(fileTag)
+    createTopScoresTxt(roiPath, locationArr, scoreArr, stateNameList, roiWidth)
+    if verbose: print("    Time:", time() - tRoi, flush=True)
     else: print("\t[Done]", flush=True)
 
     # Removing the expected frequency array
     remove(Path(expFreqPath))
 
 
 def readInData(outputDirPath):
@@ -46,35 +45,23 @@
     Reads all the epilogos score files in and combines them into a numpy array ordered by location
 
     Input:
     outputDirPath -- Path to the epilogos output directory (this contains the score files)
 
     Output:
     locationArr -- Numpy array containing the genomic locations for all the scores
-    scoreArr.sum(axis=1) -- Numpy array containing sums of the KL-Scores for each genomic bin
-    maxScoreArr -- Numpy array containing the state which had the highest KL-score in each bin
+    scoreArr    -- Numpy array containing the KL-Scores for each genomic bin
     """
     results = map(unpackNPZ, outputDirPath.glob("temp_scores_*.npz"))
 
     # Split up read results into tuples of chromosomes, scores, and locations
     dataChunks = list(zip(*results))
 
     # Figuring out chromosome order
-    rawChrNamesInts = []
-    rawChrNamesStrs = []
-    for chromosome in dataChunks[0]:
-        try:
-            rawChrNamesInts.append(int(chromosome.split("chr")[-1]))
-        except ValueError:
-            rawChrNamesStrs.append(chromosome.split("chr")[-1])
-    rawChrNamesInts.sort()
-    rawChrNamesStrs.sort()
-    chrOrder = rawChrNamesInts + rawChrNamesStrs
-    for i in range(len(chrOrder)):
-        chrOrder[i] = "chr" + str(chrOrder[i])
+    chrOrder = orderChromosomes(dataChunks[0])
 
     # Sorting the dataframes by chromosomal location
     # Creating array of scores and locations ordered by chromosome based on the read in chunks
     index = dataChunks[0].index(chrOrder[0])
     scoreArr = dataChunks[1][index]
     locationArr = dataChunks[2][index]
     for chrName in chrOrder[1:]:
@@ -82,68 +69,78 @@
         scoreArr = np.concatenate((scoreArr, dataChunks[1][index]))
         locationArr = np.concatenate((locationArr, dataChunks[2][index]))
 
     # Cleaning up the temp files after we've read them
     for file in outputDirPath.glob("temp_scores_*.npz"):
         remove(file)
 
-    maxScoreArr = np.abs(np.argmax(np.abs(np.flip(scoreArr, axis=1)), axis=1) - scoreArr.shape[1]).astype(int)
-
-    return locationArr, scoreArr.sum(axis=1), maxScoreArr
+    return locationArr, scoreArr
 
 
 def unpackNPZ(file):
     """
     Takes in an .npz file containing scores and returns the individual numpy arrays
 
     Input:
     file -- The .npz file to unpack
 
     Output:
-    npzFile['chrName'][0] -- The name of the chromosome which the scores are of
-    npzFile['scoreArr'] -- Numpy array containing the kullback leibler scores
+    npzFile['chrName'][0]  -- The name of the chromosome which the scores are of
+    npzFile['scoreArr']    -- Numpy array containing the kullback leibler scores
     npzFile['locationArr'] -- Numpy array containing the genomic locations for all the scores
     """
-    npzFile = np.load(Path(file))
+    npzFile = np.load(Path(file), allow_pickle=True)
     return npzFile['chrName'][0], npzFile['scoreArr'], npzFile['locationArr']
 
 
-def createTopScoresTxt(filePath, locationArr, scoreArr, maxScoreArr, nameArr):
+def createTopScoresTxt(filePath, locationArr, scoreArr, nameArr, roiWidth):
     """
-    Finds the top 1000 scoring bins and merges adjacent bins, then outputs a txt containing these top scoring regions and
-    some information about each (chromosome, bin start, bin end, state name, absolute value of score, sign of score)
+    Finds the top 100 regions of interest using filter-region's maxmean algorithm then outputs them in a txt with some
+    information about each (chromosome, bin start, bin end, state name, absolute value of score, sign of score)
 
     Input:
-    filePath -- The path of the file to write to
+    filePath    -- The path of the file to write to
     locationArr -- Numpy array containing the genomic locations of all the bins
-    scoreArr -- Numpy array containing the sum of the scores within each bin
-    maxScoreArr -- Numpy array containing the states which had the highest score in each bin
-    nameArr -- Numpy array containing the names of all the states
-    """
-    with open(filePath, 'w') as f:
-        # Sort the values
-        indices = (-np.abs(scoreArr)).argsort()[:1000]
-
-        locations = pd.DataFrame(np.concatenate((locationArr[indices], scoreArr[indices].reshape(len(indices), 1),
-                                                 maxScoreArr[indices].reshape(len(indices), 1)), axis=1),
-                                 columns=["Chromosome", "Start", "End", "Score", "MaxScoreLoc"])\
-                      .astype({"Chromosome": str, "Start": np.int32, "End": np.int32, "Score": np.float32,
-                               "MaxScoreLoc": np.int32})
-
-        # Iterate until all is merged
-        locations = mergeAdjacent(pr.PyRanges(locations))
-        if "Start_b" in locations.columns:
-            locations.drop(columns=["Start_b", "End_b"], inplace=True)
+    scoreArr    -- Numpy array containing the scores within each bin
+    nameArr     -- Numpy array containing the names of all the states
+    roiWidth    -- size of regions of interest in bins
 
-        # Sort by absolute value of score
-        locations = locations.iloc[(-locations["Score"].abs()).argsort()]
+    Output:
+    regionsOfInterest*.txt of top 100 regions of interest formatted as follows:
+        Column 1: Chromosome
+        Column 2: Start coordinate
+        Column 3: End coordinate
+        Column 4: Name of the largest scoring state
+        Column 5: Sum of the Kullback-Leibler scores
+        Column 6: Sign of the sum of Kullback-Leibler scores
+    """
+    with open(filePath, 'w') as outFile:
+        # Concatenate the location and score arrays so that filter regions outputs the region coords as well as scores
+        rois, indices = maxMean(np.concatenate((locationArr, scoreArr.sum(axis=1).reshape(len(scoreArr), 1)), axis=1),
+                                roiWidth, 100)
+
+        # Generating array of all indices for vectorized calculations
+        roiIndicesArr = generateROIIndicesArr(indices, roiWidth)
+
+        # Calculate the maximum contributing state in each region
+        # In the case of a tie, the higher number state wins (e.g. last state wins if all states are 0)
+        # Flip makes it so tie leads to the higher number state
+        # Calculate the maximum value for each state in and then from there the argmax for the max state
+        # Subtract from the shape of the array to reverse the effect of flip and get the state number
+        maxStates = scoreArr.shape[1] - np.argmax(np.max(np.flip(scoreArr[roiIndicesArr], axis=2), axis=1), axis=1)
+
+        # Build pandas dataframe for writing
+        locations = pd.DataFrame(rois.loc[:, ["Chromosome", "Start", "End", "Score"]])\
+            .astype({"Chromosome": str, "Start": np.int64, "End": np.int64, "Score": np.float32})
+        locations["MaxScoreState"] = maxStates.astype(np.int32)
 
         # Write all the locations to the file
         outTemplate = "{0[0]}\t{0[1]}\t{0[2]}\t{1}\t{2:.5f}\t{3}\n"
         outString = "".join(outTemplate.format(locations.iloc[i], nameArr[int(float(locations.iloc[i, 4])) - 1],
                             abs(float(locations.iloc[i, 3])), findSign(float(locations.iloc[i, 3])))
-                            for i in range(min((locations.shape[0], 100))))
-        f.write(outString)
+                            for i in range(locations.shape[0]))
+
+        outFile.write(outString)
 
 
 if __name__ == "__main__":
-    main(argv[1], argv[2], argv[3], argv[4], strToBool(argv[5]))
+    main(argv[1], argv[2], argv[3], argv[4], int(argv[5]), strToBool(argv[6]))
```

### Comparing `epilogos-0.1.1/epilogos/helpers.py` & `epilogos-0.1.2/epilogos/helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import gzip
 from time import time
 import pandas as pd
 import numpy as np
 from pathlib import Path
-
+import re
+from epilogos.filter_regions import Filter
 
 def getNumStates(stateFile):
     """
     Input:
     stateFile -- tsv containing information on all the states in the state model
 
     Output:
@@ -72,88 +73,103 @@
     """
     while True:
         b = file.read(size)
         if not b: break
         yield b
 
 
-def splitRows(dataFilePath, numProcesses):
+def countRows(dataFilePath):
     """
-    Determines what rows to assign to each core
+    Determines the number of rows in a file
 
     Input:
-    dataFilePath -- the data file which we want to chunk up and send to seperate cores
-    numProcesses -- the number of cores which we want to work over
+    dataFilePath -- the data file for which we want to count rows
 
     Output:
-    A list of tuples which contain the first and last rows for each core to use
+    totalRows -- the number of rows in in the datafile
     """
+
     # Calculate the number of rows in the input file
     if dataFilePath.name.endswith("gz"):
         with gzip.open(dataFilePath, "rb") as f:
             totalRows = sum(bl.count(b'\n') for bl in blocks(f))
     else:
         with open(dataFilePath, "rb") as f:
             totalRows = sum(bl.count(b'\n') for bl in blocks(f))
 
+    return totalRows
+
+
+def splitRows(totalRows, numProcesses):
+    """
+    Determines what rows of a datafile to assign to each core
+
+    Input:
+    totalRows    -- the number of rows we want to split between cores
+    numProcesses -- the number of cores which we want to work over
+
+    Output:
+    A list of tuples which contain the first and last rows for each core to use
+    """
     # Split the rows up according to the number of cores we have available
     # Row list contain tuples of the first and last rows to be assigned to each core
     rowList = []
     for i in range(numProcesses):
-        rowsToCalc = (i * totalRows // numProcesses, (i+1) * totalRows // numProcesses)
+        rowsToCalc = (i * totalRows // numProcesses, (i + 1) * totalRows // numProcesses)
         rowList.append(rowsToCalc)
 
     return rowList
 
 
-def readStates(file1Path=Path("null"), file2Path=Path("null"), rowsToCalc=(0, 0), expBool=True, verbose=True, groupSize=-1):
+def readStates(file1Path=Path("null"), file2Path=Path("null"), rowsToCalc=(0, 0), expBool=True, verbose=True,
+               groupSize=-1):
     """
     Reads the states from the relevant rows of the inputed data file(s)
 
     Input:
-    file1Path -- The path to the first file to read from (used in both single and paired epilogos) [default=Path("null")]
-    file2Path -- The path to the second file to read from (used only in paired epilogos) [default=Path("null")]
+    file1Path  -- The path to the first file to read from (used in both single and paired) [default=Path("null")]
+    file2Path  -- The path to the second file to read from (used only in paired epilogos) [default=Path("null")]
     rowsToCalc -- The first and last rows to read from the files [default=(0, 0)]
-    expBool -- Tells us if we are calculating the expected frequencies or the scores [default=True]
-    verbose -- If True, we print out updates [default=True]
-    groupSize -- When returning null output, return 2 evenly sized groups of this size
+    expBool    -- Tells us if we are calculating the expected frequencies or the scores [default=True]
+    verbose    -- If True, we print out updates [default=True]
+    groupSize  -- When returning null output, return 2 evenly sized groups of this size
 
     Output:
         Single Epilogos:
-            file1Arr -- 2d numpy array of the state info for each epigenome in the data file over the relevant rows
+            file1Arr    -- 2d numpy array of the state info for each epigenome in the data file over the relevant rows
         Paired Epilogos Expected Frequency:
             combinedArr -- 2d numpy array of the state info for each epigenome of both data files over the relevant rows
         Paired Epilogos Scores:
-            file1Arr -- 2d numpy array of the state info for each epigenome in the first data file over the relevant rows
-            file2Arr -- 2d numpy array of the state info for each epigenome in the second data file over the relevant rows
-            shuffledCombinedArr[:, :file1Arr.shape[1]] -- 2d numpy array of the state info shuffled between first and second
+            file1Arr    -- 2d numpy array of the state info for each epigenome in the 1st data file over relevant rows
+            file2Arr    -- 2d numpy array of the state info for each epigenome in the 2nd data file over relevant rows
+            shuffledCombinedArr[:, :file1Arr.shape[1]] -- 2d numpy array of the state info shuffled between 1st and 2nd
                                                           data files, with the same width as file1Arr
-            shuffledCombinedArr[:, file1Arr.shape[1]:] -- 2d numpy array of the state info shuffled between first and second
+            shuffledCombinedArr[:, file1Arr.shape[1]:] -- 2d numpy array of the state info shuffled between 1st and 2nd
                                                           data files, with the same width as file2Arr
     """
     # Read in the data from file 1
     if verbose and rowsToCalc[0] == 0: print("Reading data from file 1...", flush=True); tRead1 = time()
     # Dont want to read in locations
     cols = range(3, pd.read_table(file1Path, nrows=1, header=None, sep="\t").shape[1])
     # Read using pd.read_table and convert to numpy array for faster calculation (faster than np.genfromtext())
     file1Arr = pd.read_table(file1Path, usecols=cols, skiprows=rowsToCalc[0],
-                             nrows=rowsToCalc[1]-rowsToCalc[0], header=None, sep="\t").to_numpy(dtype=int) - 1
+                             nrows=rowsToCalc[1] - rowsToCalc[0], header=None, sep="\t").to_numpy(dtype=int) - 1
     if verbose and rowsToCalc[0] == 0: print("    Time: ", time() - tRead1, flush=True)
 
     # If we are doing single group epilogos, just return the data array, otherwise, we continute to the second file
     if str(file2Path) == "null":
         return file1Arr
 
     # Read in the data from file 2
     if verbose and rowsToCalc[0] == 0: print("Reading data from file 2...", flush=True); tRead2 = time()
     # Dont want to read in locations
     cols = range(3, pd.read_table(file2Path, nrows=1, header=None, sep="\t").shape[1])
     # Read using pd.read_table and convert to numpy array for faster calculation (faster than np.genfromtext())
     file2Arr = pd.read_table(file2Path, usecols=cols, skiprows=rowsToCalc[0],
-                             nrows=rowsToCalc[1]-rowsToCalc[0], header=None, sep="\t").to_numpy(dtype=int) - 1
+                             nrows=rowsToCalc[1] - rowsToCalc[0], header=None, sep="\t").to_numpy(dtype=int) - 1
     if verbose and rowsToCalc[0] == 0: print("    Time: ", time() - tRead2, flush=True)
 
     # Combining the arrays for per row shuffling
     if verbose and rowsToCalc[0] == 0: print("Combining input matrices..."); tCombine = time()
     combinedArr = np.concatenate((file1Arr, file2Arr), axis=1)
     if verbose and rowsToCalc[0] == 0: print("    Time:", time() - tCombine, flush=True)
 
@@ -168,10 +184,144 @@
     shuffledCombinedArr = np.take_along_axis(combinedArr, randomIndices, axis=1)
     if verbose and rowsToCalc[0] == 0: print("    Time:", time() - tShuffle, flush=True)
 
     # In the case of calculating the scores for pairwise epilogos,
     # we need the original file 1 and file 2 arrays as well as their shuffled counterparts
     # shuffledCombinedArr is split by size of the original arrays
     if groupSize == -1:
-        return file1Arr, file2Arr, shuffledCombinedArr[:, :file1Arr.shape[1]], shuffledCombinedArr[:, file1Arr.shape[1]:]
+        return file1Arr, file2Arr, shuffledCombinedArr[:, :file1Arr.shape[1]],\
+            shuffledCombinedArr[:, file1Arr.shape[1]:]
+    else:
+        return file1Arr, file2Arr, shuffledCombinedArr[:, :groupSize], shuffledCombinedArr[:, groupSize:2 * groupSize]
+
+
+def generateRegionArr(query):
+    """
+    Takes in one or more query regions and builds an 2 numpy array containing their coordinates.
+    Used to handle both single queries and files containing multiple queries
+
+    Input:
+    query -- Query coordinates formatted chr:start-end OR
+             Path to bed file containing query coordinates on each line, formatted chr[tab]start[tab]end
+
+    Output:
+    2D Numpy array with the first dimension being query regions and the second dimension being coordinates
+    """
+
+    # if its a single query build a one coord array
+    if re.fullmatch("chr[a-zA-z\\d]+:[\\d]+-[\\d]+", query):
+        chr = query.split(":")[0]
+        start = query.split(":")[1].split("-")[0]
+        end = query.split(":")[1].split("-")[1]
+        return np.array([[chr, int(start), int(end)]], dtype=object)
+    # if it is a path to a file, build a numpy array with all coords
+    elif Path(query).is_file():
+        return pd.read_table(Path(query), sep="\t", header=None, usecols=[0, 1, 2]).to_numpy(dtype=object)
+    else:
+        raise ValueError("Please input valid query (region formatted as chr:start-end"
+                         + "or path to bed file containing query regions)")
+
+
+def orderChromosomes(chromosomes):
+    """
+    Takes in an unordered iterable of chromosomes and orders them first by number then alphabetically
+    e.g. For humans: 1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,X,Y
+
+    Input:
+    chromosomes -- An iterable of strings containing chromosome names formatted chr[] ([] is replaced with the chr name)
+
+    Output:
+    chrOrder -- The ordered list of chromosomes
+    """
+
+    # Orders chromosomes so numbers count up, followed by alphabetical
+    rawChrNamesInts = []
+    rawChrNamesStrs = []
+    for chromosome in chromosomes:
+        try:
+            rawChrNamesInts.append(int(chromosome.split("chr")[-1]))
+        except ValueError:
+            rawChrNamesStrs.append(chromosome.split("chr")[-1])
+    rawChrNamesInts.sort()
+    rawChrNamesStrs.sort()
+    chrOrder = rawChrNamesInts + rawChrNamesStrs
+    for i in range(len(chrOrder)):
+        chrOrder[i] = "chr" + str(chrOrder[i])
+
+    return chrOrder
+
+
+def maxMean(inputArr, roiWidth, maxRegions):
+    """
+    Wrapper function for the filter-regions maxmean function. Generates 100 results and sorts them in descending order
+
+    Input:
+    inputArr   -- A numpy array containing coordinates in the first 3 columns and score metric in the 4th column
+    roiWidth   -- The desired width of the regions of interest in bins
+    maxReginos -- The number of regions for the maxmean algorithm to find
+
+    Output:
+    rois      -- Pandas dataframe containing the regions chosen by maxmean
+    indices   -- The original indices within the inputArr for the center of each of the chosen regions
+    """
+    f = Filter(method='maxmean', input=inputArr, input_type='bedgraph', aggregation_method='max',
+                  window_bins=roiWidth, max_elements=maxRegions, preserve_cols=True, quiet=False)
+    f.read()
+    f.filter()
+    rois = f.output_df
+    rois = rois.sort_values(by=["RollingMax", "RollingMean", "Score"], ascending=False).reset_index(drop=True)
+    indices = rois["OriginalIdx"].to_numpy()
+
+    return rois, indices
+
+
+def generateROIIndicesArr(indices, roiWidth):
+    """
+    Creates a 2d numpy array containing the full indices [start...end] for each region chosen by maxmean
+
+    Input:
+    indices  -- The index of the centerpoint for each region of interest
+    roiWidth -- The width of each region of interest in bins
+
+    Output:
+    np.array(upperLower, dtype=np.int32) -- 2D numpy array with the 1st dimension being regions
+                                            and the 2nd dimension being all the indices within each region
+    """
+    upperLower = []
+    for idx in indices:
+        # If the region of interest is an odd number of bins we have to add 1 to the upper index
+        lowerIdx = idx - roiWidth // 2
+        upperIdx = idx + roiWidth // 2
+        if roiWidth % 2: upperIdx += 1
+        upperLower.append(np.arange(lowerIdx, upperIdx, dtype=np.int32))
+    return np.array(upperLower, dtype=np.int32)
+
+
+def findSign(x):
+    """
+    Returns a string containing the sign of the inputted number
+
+    Input:
+    x -- Any number
+
+    Output:
+    "+" or "-"
+    """
+    if (x >= 0):
+        return "+"
     else:
-        return file1Arr, file2Arr, shuffledCombinedArr[:, :groupSize], shuffledCombinedArr[:, groupSize:2*groupSize]
+        return "-"
+
+
+def sharedToNumpy(sharedArr, numRows, numStates):
+    """
+    Helper for unflattening a shared array into a 2d numpy array
+
+    Input:
+    sharedArr -- The shared array to shape
+    numRows   -- The number of rows for the numpy array
+    numStates -- The number of columns for the numpy array
+
+    Output:
+    numpy array generated from a buffered shared array
+    """
+    return np.frombuffer(sharedArr, dtype=np.float32).reshape((numRows, numStates))
```

### Comparing `epilogos-0.1.1/epilogos/pairwiseVisual.py` & `epilogos-0.1.2/epilogos/roiAndVisualPairwise.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,178 +7,204 @@
 import warnings
 from time import time
 import gzip
 from multiprocessing import cpu_count, Pool
 from contextlib import closing
 from itertools import repeat
 from os import remove
-import pyranges as pr
 from statsmodels.stats.multitest import multipletests
-from epilogos.helpers import strToBool, getStateNames, getStateColorsRGB, getNumStates
+from epilogos.helpers import maxMean, generateROIIndicesArr, orderChromosomes, strToBool, getStateNames,\
+    getStateColorsRGB, getNumStates, findSign
 
 
-def main(group1Name, group2Name, stateInfo, outputDir, fileTag, numProcesses, diagnosticBool, numTrials, samplingSize,
-         expFreqPath, verbose):
+def main(group1Name, group2Name, stateInfo, outputDir, fileTag, numProcesses, pvalBool, diagnosticBool, numTrials,
+         samplingSize, expFreqPath, roiWidth, verbose):
     """
-    Takes in the scores for the 2 paired groups and finds the distance between them. Then fits a gennorm distribution to the
-    distances between the null scores and uses this to calculate the pvalues of the distances. These pvalues are written out,
-    used to generate txt file of most interesting loci, and used to create manhattan plots of the genome.
-
-    Input:
-    group1Name -- String of the name of the first epilogos group
-    group2Name -- String of the name of the second epilogos group
-    stateInfo -- State model tab seperated information file
-    outputDir -- The output directory for epilogos
-    fileTag -- A string which helps ensure outputed files are named similarly within an epilogos run
-    numProcesses -- The number of cores which to run on
-    diagnosticBool -- Boolean which if True tells us to generate diagnostic plots of the gennorm fit on the null data and
-                      comparisons between the null and real data
-    numTrials -- The number of gennorm fits to do
-    samplingSize -- The amount of null data to fit
-    expFreqPath -- The location of the stored expected frequency array
-    verbose -- Boolean which if True, causes much more detailed prints
+    Takes in the scores for the 2 paired groups and finds the distance between them. Then fits a gennorm distribution to
+    the distances between the null scores and uses this to calculate the pvalues of the distances. These pvalues are
+    written out, used to generate txt file of most interesting loci, and used to create manhattan plots of the genome.
+
+    Input:
+    group1Name     -- String of the name of the first epilogos group
+    group2Name     -- String of the name of the second epilogos group
+    stateInfo      -- State model tab seperated information file
+    outputDir      -- The output directory for epilogos
+    fileTag        -- A string which helps ensure outputed files are named similarly within an epilogos run
+    numProcesses   -- The number of cores which to run on
+    pvalBool       -- Boolean which if True tells epilogos to generate pvalues for pairwise scores
+    diagnosticBool -- Boolean which if True tells us to generate diagnostic plots of the gennorm fit on the null data
+                      and comparisons between the null and real data
+    numTrials      -- The number of gennorm fits to do
+    samplingSize   -- The amount of null data to fit
+    expFreqPath    -- The location of the stored expected frequency array
+    roiWidth       -- size of regions of interest in bins
+    verbose        -- Boolean which if True, causes much more detailed prints
     """
     tTotal = time()
 
     outputDirPath = Path(outputDir)
-    np.random.seed(7032016)
 
     # Plotting setting
     plt.rcParams['agg.path.chunksize'] = 10000
 
     numStates = getNumStates(stateInfo)
     stateColorList = getStateColorsRGB(stateInfo)
     stateNameList = getStateNames(stateInfo)
 
     # If user doesn't want to choose number of cores use as many as available
     if numProcesses == 0:
         numProcesses = cpu_count()
 
-    # Fitting a gennorm distribution to the distances
-    if verbose: print("\nFitting gennorm distribution to distances...", flush=True); tFit = time()
-    else: print("    Fitting distances\t", end="", flush=True)
-    params, distanceArrNull, nonQuiescentIdx = fitDistances(outputDirPath, numProcesses, numTrials, samplingSize)
-    if verbose: print("    Time:", time() - tFit, flush=True)
-    else: print("\t[Done]", flush=True)
+    if pvalBool:
+        # Fitting a gennorm distribution to the distances
+        if verbose: print("\nFitting gennorm distribution to distances...", flush=True); tFit = time()
+        else: print("    Fitting distances\t", end="", flush=True)
+        params, distanceArrNull, nonQuiescentIdx = fitDistances(outputDirPath, numProcesses, numTrials, samplingSize)
+        if verbose: print("    Time:", time() - tFit, flush=True)
+        else: print("\t[Done]", flush=True)
 
     # Read in observation files
     if verbose: print("Reading in observation files...", flush=True); tRead = time()
     else: print("    Reading in files\t", end="", flush=True)
     locationArr, distanceArrReal, maxDiffArr, chrDict = readInData(outputDirPath, numProcesses, numStates)
     if verbose: print("    Time:", time() - tRead, flush=True)
     else: print("\t[Done]", flush=True)
 
-    # Splitting the params up
-    beta, loc, scale = params[:-2], params[-2], params[-1]
+    if pvalBool:
+        # Splitting the params up
+        beta, loc, scale = params[:-2], params[-2], params[-1]
+
+        # Creating Diagnostic Figures
+        if diagnosticBool:
+            if verbose: print("Creating diagnostic figures...", flush=True); tDiagnostic = time()
+            else: print("    Diagnostic figures\t", end="", flush=True)
+            createDiagnosticFigures(distanceArrReal, distanceArrNull, nonQuiescentIdx, beta, loc, scale, outputDirPath,
+                                    fileTag)
+            if verbose: print("    Time:", time() - tDiagnostic, flush=True)
+            else: print("\t[Done]", flush=True)
+
+        # Calculating PValues
+        if verbose: print("Calculating P-Values...", flush=True); tPVal = time()
+        else: print("    Calculating p-vals\t", end="", flush=True)
+        pvals = calculatePVals(distanceArrReal, beta, loc, scale)
+        if verbose: print("    Time:", time() - tPVal, flush=True)
+        else: print("\t[Done]", flush=True)
 
-    # Creating Diagnostic Figures
-    if diagnosticBool:
-        if verbose: print("Creating diagnostic figures...", flush=True); tDiagnostic = time()
-        else: print("    Diagnostic figures\t", end="", flush=True)
-        createDiagnosticFigures(distanceArrReal, distanceArrNull, nonQuiescentIdx, beta, loc, scale, outputDirPath, fileTag)
-        if verbose: print("    Time:", time() - tDiagnostic, flush=True)
+        # Perform multiple hypothesis correction on pvals
+        if verbose: print("Performing Benjamini-Hochberg procedure...", flush=True); tMH = time()
+        else: print("    Benjamini-Hochberg procedure\t", end="", flush=True)
+        mhPvals = multipletests(pvals, method="fdr_bh")[1]
+        if verbose: print("    Time:", time() - tMH, flush=True)
         else: print("\t[Done]", flush=True)
 
-    # Calculating PValues
-    if verbose: print("Calculating P-Values...", flush=True); tPVal = time()
-    else: print("    Calculating p-vals\t", end="", flush=True)
-    pvals = calculatePVals(distanceArrReal, beta, loc, scale)
-    if verbose: print("    Time:", time() - tPVal, flush=True)
-    else: print("\t[Done]", flush=True)
+    else:
+        # Calculate the absolute value of zcores for creating the manhattan plots
+        if verbose: print("Calculating Z-Scores...", flush=True); tZS = time()
+        else: print("    Z-Scores\t", end="", flush=True)
+        zScores = np.abs(st.zscore(distanceArrReal))
+        if verbose: print("    Time:", time() - tZS, flush=True)
+        else: print("\t[Done]", flush=True)
 
     # Create an output file which summarizes the results
     if verbose: print("Writing metrics file...", flush=True); tMetrics = time()
     else: print("    Writing metrics\t", end="", flush=True)
-    writeMetrics(locationArr, chrDict, maxDiffArr, distanceArrReal, pvals, outputDirPath, fileTag)
+    if pvalBool:
+        writeMetrics(locationArr, chrDict, maxDiffArr, stateNameList, distanceArrReal, outputDirPath, fileTag, pvalBool,
+                     pvals=pvals, mhPvals=mhPvals)
+    else:
+        writeMetrics(locationArr, chrDict, maxDiffArr, stateNameList, distanceArrReal, outputDirPath, fileTag, pvalBool)
     if verbose: print("    Time:", time() - tMetrics, flush=True)
     else: print("\t[Done]", flush=True)
 
-    # Perform multiple hypothesis correction on pvals
-    if verbose: print("Performing Benjamini-Hochberg procedure...", flush=True); tMH = time()
-    else: print("    Benjamini-Hochberg procedure\t", end="", flush=True)
-    mhPvals = multipletests(pvals, method="fdr_bh")[1]
-    if verbose: print("    Time:", time() - tMH, flush=True)
-    else: print("\t[Done]", flush=True)
-
-    # Create txt file of top 1000 loci with adjacent merged
-    if verbose: print("Creating .txt file of top loci...", flush=True); t1000 = time()
-    else: print("    Greatest hits txt\t", end="", flush=True)
-    roiPath = outputDirPath / "greatestHits_{}.txt".format(fileTag)
-    createTopScoresTxt(roiPath, locationArr, chrDict, distanceArrReal, maxDiffArr, stateNameList, pvals, False, mhPvals)
-    if verbose: print("    Time:", time() - t1000, flush=True)
-    else: print("\t[Done]", flush=True)
+    if pvalBool:
+        # Create txt file of significant loci with adjacent merged
+        if verbose: print("Creating .txt file of top loci...", flush=True); tGreat = time()
+        else: print("    Regions of interest txt\t", end="", flush=True)
+        roiPath = outputDirPath / "regionsOfInterest_{}.txt".format(fileTag)
+        createROITxt(roiPath, locationArr, chrDict, distanceArrReal, maxDiffArr, stateNameList, pvals, mhPvals,
+                     roiWidth)
+        if verbose: print("    Time:", time() - tGreat, flush=True)
+        else: print("\t[Done]", flush=True)
 
-    # Create txt file of significant loci
-    if verbose: print("Creating .txt file of significant loci...", flush=True); tSig = time()
-    else: print("    Significant loci txt\t", end="", flush=True)
-    roiPath = outputDirPath / "significantLoci_{}.txt.gz".format(fileTag)
-    createTopScoresTxt(roiPath, locationArr, chrDict, distanceArrReal, maxDiffArr, stateNameList, pvals, True, mhPvals)
-    if verbose: print("    Time:", time() - tSig, flush=True)
-    else: print("\t[Done]", flush=True)
+        # Create txt file of significant loci
+        if verbose: print("Creating .txt file of significant loci...", flush=True); tSig = time()
+        else: print("    Significant loci txt\t", end="", flush=True)
+        roiPath = outputDirPath / "significantLoci_{}.txt.gz".format(fileTag)
+        createSignificantLociTxt(roiPath, locationArr, chrDict, distanceArrReal, maxDiffArr, stateNameList, pvals,
+                                 mhPvals)
+        if verbose: print("    Time:", time() - tSig, flush=True)
+        else: print("\t[Done]", flush=True)
+    else:
+        if verbose: print("Creating .txt file of top loci...", flush=True); tGreat = time()
+        else: print("    Regions of interest txt\t", end="", flush=True)
+        roiPath = outputDirPath / "regionsOfInterest_{}.txt".format(fileTag)
+        createROINoSignificance(roiPath, locationArr, chrDict, distanceArrReal, maxDiffArr, stateNameList, zScores,
+                                roiWidth)
+        if verbose: print("    Time:", time() - tGreat, flush=True)
+        else: print("\t[Done]", flush=True)
 
     # Create Chromosome Manhattan Plot
     if verbose: print("Creating Individual Chromosome Manhattan Plots", flush=True); tCManhattan = time()
     else: print("    Chromosome Manhattan\t", end="", flush=True)
-    createChromosomeManhattan(group1Name, group2Name, locationArr, chrDict, distanceArrReal, maxDiffArr, params,
-                              stateColorList, outputDirPath, fileTag, numProcesses, mhPvals)
+    if pvalBool:
+        createChromosomeManhattan(group1Name, group2Name, locationArr, chrDict, distanceArrReal, maxDiffArr,
+                                  stateColorList, outputDirPath, fileTag, numProcesses, pvalBool, params=params,
+                                  mhPvals=mhPvals)
+    else:
+        createChromosomeManhattan(group1Name, group2Name, locationArr, chrDict, distanceArrReal, maxDiffArr,
+                                  stateColorList, outputDirPath, fileTag, numProcesses, pvalBool, zScores=zScores)
     if verbose: print("    Time:", time() - tCManhattan, flush=True)
     else: print("\t[Done]", flush=True)
 
     # Create Genome Manhattan Plot
     if verbose: print("Creating Genome-Wide Manhattan Plot", flush=True); tGManhattan = time()
     else: print("    Genome-wide Manhattan\t", end="", flush=True)
-    createGenomeManhattan(group1Name, group2Name, locationArr, chrDict, distanceArrReal, maxDiffArr, beta, loc, scale,
-                          stateColorList, outputDirPath, fileTag, mhPvals)
+    if pvalBool:
+        createGenomeManhattan(group1Name, group2Name, locationArr, chrDict, distanceArrReal, maxDiffArr,
+                              stateColorList, outputDirPath, fileTag, pvalBool, beta=beta, loc=loc, scale=scale,
+                              mhPvals=mhPvals)
+    else:
+        createGenomeManhattan(group1Name, group2Name, locationArr, chrDict, distanceArrReal, maxDiffArr,
+                              stateColorList, outputDirPath, fileTag, pvalBool, zScores=zScores)
     if verbose: print("    Time:", time() - tGManhattan, flush=True)
     else: print("\t[Done]", flush=True)
 
     # Removing the expected frequency array
     remove(Path(expFreqPath))
 
     if verbose: print("Total Time:", time() - tTotal, flush=True)
 
 
 def fitDistances(outputDirPath, numProcesses, numTrials, samplingSize):
     """
-    Filters out quiescent bins and deploys the processes which fits the null distances. Then calculates the median fit based
-    on the negative loglikelihood function
+    Filters out quiescent bins and deploys the processes which fits the null distances.
+    Then calculates the median fit based on the negative loglikelihood function
 
     Input:
     outputDirPath -- Path to the epilogos output directory (this contains the score files)
-    numProcesses -- The number of cores to run on
-    numTrials -- The number of fits to do
-    samplingSize -- The amount of data to fit each time
+    numProcesses  -- The number of cores to run on
+    numTrials     -- The number of fits to do
+    samplingSize  -- The amount of data to fit each time
 
     Output:
-    (fitDF.iloc[medianIndex, 0], fitDF.iloc[medianIndex, 1], fitDF.iloc[medianIndex, 2]) -- Tuple with beta, loc, and scale
+    (fitDF.iloc[medianIndex, 0], fitDF.iloc[medianIndex, 1], fitDF.iloc[medianIndex, 2]) -- Tuple with beta, loc, scale
                                                                                             params of the median fit
     distanceArrNull -- Numpy array of the null distances
     nonQuiescentIdx -- indices of non-quiescent bins (specifically used for distance arrays)
     """
     # Filtering out quiescent values (When there are exactly zero differences between both score arrays)
 
     with closing(Pool(numProcesses)) as pool:
         results = pool.starmap(readNull, zip(outputDirPath.glob("temp_nullDistances_*.npz"),
                                              outputDirPath.glob("temp_quiescence_*.npz")))
     pool.join()
 
     # Figuring out chromosome order
     chromosomes = list(zip(*list(zip(*results))[0]))[0]
-    rawChrNamesInts = []
-    rawChrNamesStrs = []
-    for chromosome in chromosomes:
-        try:
-            rawChrNamesInts.append(int(chromosome.split("chr")[-1]))
-        except ValueError:
-            rawChrNamesStrs.append(chromosome.split("chr")[-1])
-    rawChrNamesInts.sort()
-    rawChrNamesStrs.sort()
-    chrOrder = rawChrNamesInts + rawChrNamesStrs
-    for i in range(len(chrOrder)):
-        chrOrder[i] = "chr" + str(chrOrder[i])
+    chrOrder = orderChromosomes(chromosomes)
 
     # Creating array of null distances ordered by chromosome based on the read in chunks
     nullChunks = list(zip(*list(zip(*results))[0]))
     index = nullChunks[0].index(chrOrder[0])
     distanceArrNull = nullChunks[1][index]
     for chrName in chrOrder[1:]:
         index = nullChunks[0].index(chrName)
@@ -188,71 +214,70 @@
     quiescenceChunks = list(zip(*list(zip(*results))[1]))
     index = quiescenceChunks[0].index(chrOrder[0])
     quiescenceArr = quiescenceChunks[1][index]
     for chrName in chrOrder[1:]:
         index = quiescenceChunks[0].index(chrName)
         quiescenceArr = np.concatenate((quiescenceArr, quiescenceChunks[1][index]))
 
-    nonQuiescentIdx = np.where(quiescenceArr == False)[0]
+    nonQuiescentIdx = np.where(np.invert(quiescenceArr))[0]
 
     with closing(Pool(numProcesses)) as pool:
-        results = pool.starmap(fitOnSample, zip(repeat(distanceArrNull[nonQuiescentIdx], numTrials),
-                                                repeat(samplingSize, numTrials)))
+        results = pool.starmap(fitOnSubSample, zip(repeat(distanceArrNull[nonQuiescentIdx], numTrials),
+                                                   repeat(samplingSize, numTrials)))
     pool.join()
 
     # Creating dataframe of all params and nnlf so that we can figure out median
     index = [i for i in range(numTrials)]
     columns = ["beta", "loc", "scale", "nnlf"]
     fitDF = pd.DataFrame(index=index, columns=columns)
     for i in range(len(results)):
         fitDF.iloc[i, 0] = results[i][0][0]
         fitDF.iloc[i, 1] = results[i][0][1]
         fitDF.iloc[i, 2] = results[i][0][2]
         fitDF.iloc[i, 3] = results[i][1]
     fitDF.sort_values(by=["nnlf"], inplace=True)
 
     # return params, dataReal, dataNull
-    medianIndex = int((numTrials-1)/2)
+    medianIndex = int((numTrials - 1) / 2)
     return (fitDF.iloc[medianIndex, 0], fitDF.iloc[medianIndex, 1], fitDF.iloc[medianIndex, 2]),\
-           distanceArrNull,\
-           nonQuiescentIdx
+        distanceArrNull, nonQuiescentIdx
 
 
 def readNull(nullFile, quiescenceFile):
     """
     Reads in the null scores
 
     Input:
-    nullFile -- The path to the file containing the null scores
+    nullFile       -- The path to the file containing the null scores
     quiescenceFile -- The path to the file containing T/F regarding quiescence for each bin
 
     Output:
-    (npzFile['chrName'][0], npzFile['nullDistances']) -- Tuple with the chromosome name and the null signed squared euclidean
-                                                         distances
-    (npzFileQuiescence['chrName'][0], npzFileQuiescence['quiescenceArr']) -- Tuple with chromosome name and the T/F value of
-                                                                             quiescence for each bin
+    (npzFile['chrName'][0], npzFile['nullDistances']) -- Tuple with the chromosome name and the null signed squared
+                                                         euclidean distances
+    (npzFileQuiescence['chrName'][0], npzFileQuiescence['quiescenceArr']) -- Tuple with chromosome name and the T/F
+                                                                             value of quiescence for each bin
     """
     npzFileNull = np.load(Path(nullFile))
     npzFileQuiescence = np.load(Path(quiescenceFile))
 
-    return (npzFileNull['chrName'][0], npzFileNull['nullDistances']), (npzFileQuiescence['chrName'][0],
-                                                                       npzFileQuiescence['quiescenceArr'])
+    return (npzFileNull['chrName'][0], npzFileNull['nullDistances']),\
+           (npzFileQuiescence['chrName'][0], npzFileQuiescence['quiescenceArr'])
 
 
-def fitOnSample(distanceArrNull, samplingSize):
+def fitOnSubSample(distanceArrNull, samplingSize):
     """
-    Fits a sample of the null distances
+    Fits a sub-sample of the null distances
 
     Input:
     distanceArrNull -- Numpy array containing the distances to sample for the fit
-    samplingSize -- The size of the sample to fit
+    samplingSize    -- The size of the sample to fit
 
     Output:
     params -- The fit parameters obtained
-    nnlf -- The negative loglikelihood function obtained by the fit
+    nnlf   -- The negative loglikelihood function obtained by the fit
     """
     if len(distanceArrNull) <= samplingSize:
         sampleData = distanceArrNull
     else:
         np.random.seed()  # On linux, multiprocessing inherits the master seed and doesn't generate fully random numbers
         sampleData = pd.Series(np.random.choice(distanceArrNull, size=samplingSize, replace=False))
 
@@ -271,22 +296,22 @@
 
 def readInData(outputDirPath, numProcesses, numStates):
     """
     Reads all the epilogos score files in and combines them into a numpy array ordered by location
 
     Input:
     outputDirPath -- Path to the epilogos output directory (this contains the score files)
-    numProcesses -- The number of cores used to read in score files
-    numStates -- The number of states in the state model
+    numProcesses  -- The number of cores used to read in score files
+    numStates     -- The number of states in the state model
 
     Output:
-    locationArr -- Numpy array containing the genomic locations for all the scores
+    locationArr     -- Numpy array containing the genomic locations for all the scores
     distanceArrReal -- Numpy array containing binwise signed squared euclidean distances of the scores of the two groups
-    maxDiffArr -- Numpy array containing the state which had the absolute distance in each bin
-    chrDict -- Dictionary containing mappings between number values and chromosome names (helps locationArr use less memory)
+    maxDiffArr      -- Numpy array containing the state which had the absolute distance in each bin
+    chrDict         -- Dictionary containing mappings between number values and chromosome names (helps use less memory)
     """
     # For keeping the data arrays organized correctly
     realNames = ["chr", "binStart", "binEnd"] + ["s{}".format(i) for i in range(1, numStates + 1)]
 
     # Data frame to dump inputed data into
     diffDF = pd.DataFrame(columns=realNames)
 
@@ -296,49 +321,40 @@
     pool.join()
 
     # Concatenating all chunks to the real differences dataframe
     for diffDFChunk in results:
         diffDF = pd.concat((diffDF, diffDFChunk), axis=0, ignore_index=True)
 
     # Figuring out chromosome order
-    chromosomes = diffDF['chr'].unique()
-    rawChrNamesInts = []
-    rawChrNamesStrs = []
-    for chromosome in chromosomes:
-        try:
-            rawChrNamesInts.append(int(chromosome.split("chr")[-1]))
-        except ValueError:
-            rawChrNamesStrs.append(chromosome.split("chr")[-1])
-    rawChrNamesInts.sort()
-    rawChrNamesStrs.sort()
-    chrOrder = rawChrNamesInts + rawChrNamesStrs
-    for i in range(len(chrOrder)):
-        chrOrder[i] = "chr" + str(chrOrder[i])
+    chrOrder = orderChromosomes(diffDF['chr'].unique())
 
     # Sorting the dataframes by chromosomal location
     diffDF["chr"] = pd.Categorical(diffDF["chr"], categories=chrOrder, ordered=True)
     diffDF.sort_values(by=["chr", "binStart", "binEnd"], inplace=True)
 
     # Creating a dictionary to make location array take less memory
     chrNumbers = [i for i in range(1, len(chrOrder) + 1)]
     chrDict    = dict(zip(chrNumbers, chrOrder))
 
     # Convert dataframes to np arrays for easier manipulation
-    locationArr = diffDF.iloc[:, 0:3].replace({"chr": dict(zip(chrOrder, chrNumbers))}).to_numpy(dtype=np.int32)
+    locationArr = diffDF.iloc[:, 0:3].replace({"chr": dict(zip(chrOrder, chrNumbers))}).to_numpy(dtype=np.int64)
     diffArr     = diffDF.iloc[:, 3:].to_numpy(dtype=np.float32)
 
     # Cleaning up the temp files after we've read them
     for file in outputDirPath.glob("temp_*.npz"):
         remove(file)
 
     # Calculate the signed squared euclidean distance array for the real data
     distanceArrReal = np.sum(np.square(diffArr), axis=1) * np.sign(np.sum(diffArr, axis=1))
 
     # Calculate the maximum contributing state for each bin
     # In the case of a tie, the higher number state wins (e.g. last state wins if all states are 0)
+    # Flip makes it so tie leads to the higher number state
+    # Calculate the maximum value for each state in and then from there the argmax for the max state
+    # Subtract from the shape of the array to reverse the effect of flip and get the state number
     maxDiffArr = np.abs(np.argmax(np.abs(np.flip(diffArr, axis=1)), axis=1) - diffArr.shape[1]).astype(np.int32)
 
     return locationArr, distanceArrReal, maxDiffArr, chrDict
 
 
 def readTableMulti(realFile, realNames):
     """
@@ -351,27 +367,34 @@
     diffDFChunk -- Pandas dataframe containing the real scores
     """
     diffDFChunk = pd.read_table(Path(realFile), header=None, sep="\t", names=realNames)
 
     return diffDFChunk
 
 
-def createDiagnosticFigures(distanceArrReal, distanceArrNull, nonQuiescentIdx, beta, loc, scale, outputDirPath, fileTag):
+def createDiagnosticFigures(distanceArrReal, distanceArrNull, nonQuiescentIdx, beta, loc, scale, outputDirPath,
+                            fileTag):
     """
     Generate diagnostic plots of the gennorm fit on the null data and comparisons between the null and real data
 
     Input:
     distanceArrReal -- Numpy array containing the real distances
     distanceArrNull -- Numpy array containing the null distances
     nonQuiescentIdx -- indices of non-quiescent bins (specifically used for distance arrays)
-    beta -- gennorm fit parameter
-    loc -- gennorm fit parameter
-    scale -- gennorm fit parameter
-    outputDirPath -- The path to the epilogos output directory
-    fileTag -- A string which helps ensure outputed files are named similarly within an epilogos run
+    beta            -- gennorm fit parameter
+    loc             -- gennorm fit parameter
+    scale           -- gennorm fit parameter
+    outputDirPath   -- The path to the epilogos output directory
+    fileTag         -- A string which helps ensure outputed files are named similarly within an epilogos run
+
+    Output:
+    Graphs depicting fit of gennorm on null data ([min, max] & [-1,1])
+    Histograms comparing real and null data ([min, max] & [-1,1])
+    Scatterplot of Real vs Null distances
+    Box Plots Showcasing fit accuracy
     """
     diagnosticDirPath = outputDirPath / "diagnosticFigures_{}".format(fileTag)
     if not diagnosticDirPath.exists():
         diagnosticDirPath.mkdir(parents=True)
 
     dataReal = pd.Series(distanceArrReal[nonQuiescentIdx])
     dataNull = pd.Series(distanceArrNull[nonQuiescentIdx])
@@ -404,32 +427,32 @@
     fig.savefig(figPath, bbox_inches='tight', dpi=400, facecolor="#FFFFFF", edgecolor="#FFFFFF", transparent=False)
     fig.clear()
     plt.close(fig)
 
     # Real Data Histogram vs. Null Data Histogram (Range=(-1, 1))
     fig = plt.figure(figsize=(16, 9))
     ax = fig.add_subplot(111)
-    dataReal.plot(kind='hist', bins=400, range=(-1, 1), density=True, alpha=0.5, label='Distances in Real Data', legend=True,
-                  ax=ax)
-    dataNull.plot(kind='hist', bins=400, range=(-1, 1), density=True, alpha=0.5, label='Distances in Null Data', legend=True,
-                  ax=ax)
+    dataReal.plot(kind='hist', bins=400, range=(-1, 1), density=True, alpha=0.5, label='Distances in Real Data',
+                  legend=True, ax=ax)
+    dataNull.plot(kind='hist', bins=400, range=(-1, 1), density=True, alpha=0.5, label='Distances in Null Data',
+                  legend=True, ax=ax)
     plt.title("Real Data vs. Null Data (range=(-1, 1))")
     figPath = diagnosticDirPath / "real_vs_null_histogram_n1to1.pdf"
     fig.savefig(figPath, bbox_inches='tight', dpi=400, facecolor="#FFFFFF", edgecolor="#FFFFFF", transparent=False)
     fig.clear()
     plt.close(fig)
 
     # Real Data Histogram vs. Null Data Histogram (Range=(-max(abs), max(abs)))
     fig = plt.figure(figsize=(16, 9))
     ax = fig.add_subplot(111)
     rangeLim = np.amax(np.abs(dataReal))
-    dataReal.plot(kind='hist', bins=400, range=(-rangeLim, rangeLim), density=True, alpha=0.5, label='Distances in Real Data',
-                  legend=True, ax=ax)
-    dataNull.plot(kind='hist', bins=400, range=(-rangeLim, rangeLim), density=True, alpha=0.5, label='Distances in Null Data',
-                  legend=True, ax=ax)
+    dataReal.plot(kind='hist', bins=400, range=(-rangeLim, rangeLim), density=True, alpha=0.5,
+                  label='Distances in Real Data', legend=True, ax=ax)
+    dataNull.plot(kind='hist', bins=400, range=(-rangeLim, rangeLim), density=True, alpha=0.5,
+                  label='Distances in Null Data', legend=True, ax=ax)
     plt.title("Real Data vs. Null Data (range=(-max(abs), max(abs)))")
     figPath = diagnosticDirPath / "real_vs_null_histogram_minToMax.pdf"
     fig.savefig(figPath, bbox_inches='tight', dpi=400, facecolor="#FFFFFF", edgecolor="#FFFFFF", transparent=False)
     fig.clear()
     plt.close(fig)
 
     # Real vs Null distance scatter plot
@@ -448,211 +471,343 @@
     # Box Plots Showcasing fit accuracy
     dist = st.gennorm.rvs(beta, loc=loc, scale=scale, size=dataNull.size)
     data = [dataNull, dist, dataReal]
     medianprops = dict(linewidth=2, color='black')
     boxprops = dict(linewidth=2, color='black')
     whiskerprops = dict(linewidth=2, color='black')
     capprops = dict(linewidth=2, color='black')
-    fig = plt.figure(figsize=(12,8))
-    bplot = plt.boxplot(data, patch_artist=True, medianprops=medianprops, boxprops=boxprops, whiskerprops=whiskerprops, capprops=capprops, showfliers=False)
+    fig = plt.figure(figsize=(12, 8))
+    bplot = plt.boxplot(data, patch_artist=True, medianprops=medianprops, boxprops=boxprops, whiskerprops=whiskerprops,
+                        capprops=capprops, showfliers=False)
     plt.xticks([1, 2, 3], ['Null', 'Fit', 'Real'])
     plt.xlabel("Data")
     plt.ylabel("Signed Squared Euclidean Distance")
 
     colors = ['#ff7f0e', '#bcbd22', '#d62728']
     for patch, color in zip(bplot['boxes'], colors):
         patch.set_facecolor(color)
 
     plt.title("Box Plots of Null and Real Data vs Fit")
-    rigPath = diagnosticDirPath / "null_vs_fit_vs_real_boxplots.pdf"
+    figPath = diagnosticDirPath / "null_vs_fit_vs_real_boxplots.pdf"
     fig.savefig(figPath, bbox_inches='tight', dpi=400, facecolor="#FFFFFF", edgecolor="#FFFFFF", transparent=False)
     fig.clear()
     plt.close(fig)
 
 
 def calculatePVals(distanceArrReal, beta, loc, scale):
     """
     Calculates the pvalues of the real distances based on the fit of the null distances
 
     Input:
     distanceArrReal -- Numpy array containing real distances
-    beta -- gennorm fit parameter
-    loc -- gennorm fit parameter
-    scale -- gennorm fit parameter
+    beta            -- gennorm fit parameter
+    loc             -- gennorm fit parameter
+    scale           -- gennorm fit parameter
 
     Output:
     pvals -- Numpy array containing pvalues of the distances
     """
     pvalsBelowLoc = 2 * st.gennorm.cdf(distanceArrReal[np.where(distanceArrReal <= loc)[0]], beta, loc=loc, scale=scale)
-    pvalsAboveLoc = 2 * (1 - st.gennorm.cdf(distanceArrReal[np.where(distanceArrReal > loc)[0]], beta, loc=loc, scale=scale))
+    pvalsAboveLoc = 2 * (1 - st.gennorm.cdf(distanceArrReal[np.where(distanceArrReal > loc)[0]], beta, loc=loc,
+                         scale=scale))
 
     pvals = np.zeros(len(distanceArrReal))
     pvals[np.where(distanceArrReal <= loc)[0]] = pvalsBelowLoc
     pvals[np.where(distanceArrReal > loc)[0]]  = pvalsAboveLoc
 
     return pvals
 
 
-def writeMetrics(locationArr, chrDict, maxDiffArr, distanceArrReal, pvals, outputDirPath, fileTag):
+def writeMetrics(locationArr, chrDict, maxDiffArr, nameArr, distanceArrReal, outputDirPath, fileTag, pvalBool,
+                 pvals=[], mhPvals=[]):
     """
     Writes metrics file to disk. Metrics file contains the following columns in order:
     chromosome, bin start, bin end, state with highest difference, signed squared euclidean distance, pvalue of distance
 
     Input:
-    locationArr -- Numpy array containing the genomic locations of all the bins
-    chrDict -- Dictionary containing mappings between number values and chromosome names (helps locationArr use less memory)
-    maxDiffArr -- Numpy array containing the states which had the largest difference between the two groups in each bin
+    locationArr     -- Numpy array containing the genomic locations of all the bins
+    chrDict         -- Dictionary containing mappings between number values and chromosome names (helps use less memory)
+    maxDiffArr      -- Numpy array containing the states which had the largest difference between the two groups in
+                       each bin
+    nameArr         -- Numpy array containing the names of all the states
     distanceArrReal -- Numpy array containing the real distances
-    pvals -- Numpy array containing the pvalues of all the distances
-    outputDirPath -- The path of the output directory for epilogos
-    fileTag -- A string which helps ensure outputed files are named similarly within an epilogos run
+    outputDirPath   -- The path of the output directory for epilogos
+    fileTag         -- A string which helps ensure outputed files are named similarly within an epilogos run
+    pvalBool        -- Boolean which if True tells epilogos to generate pvalues for pairwise scores
+    pvals           -- Numpy array containing the pvalues of all the distances
+    mhPvals         -- Multiple hypothesis corrected pvals using the Benjamini-Hochberg procedure
+
+    Output:
+    pairwiseMetrics*.txt.gz file formatted as
+        Column 1: Chromosome
+        Column 2: Start coordinate
+        Column 3: End coordinate
+        Column 4: Name of the largest difference state
+        Column 5: Squared euclidean distance between the scores
+        Column 6: Direction of the distance (sign determined by the higher signal between groups 1 and 2)
+
+    If P-values are enabled, the following columns are additionally added
+        Column 7: P-Value of the distance
+        Column 8: Benjamini–Hochberg adjusted P-Value of the distance
     """
     if not outputDirPath.exists():
         outputDirPath.mkdir(parents=True)
 
     metricsTxtPath = outputDirPath / "pairwiseMetrics_{}.txt.gz".format(fileTag)
     metricsTxt = gzip.open(metricsTxtPath, "wt")
 
     # Creating a string to write out the raw differences (faster than np.savetxt)
-    metricsTemplate = "{0[0]}\t{1[0]}\t{1[1]}\t{2}\t{3:.5f}\t{4:.5e}\n"
-    metricsStr = "".join(metricsTemplate.format(chrDict[locationArr[i, 0]], locationArr[i, 1:3], maxDiffArr[i],
-                                                distanceArrReal[i], pvals[i]) for i in range(len(distanceArrReal)))
+    if pvalBool:
+        metricsTemplate = "{0}\t{1[0]}\t{1[1]}\t{2}\t{3:.5f}\t{4}\t{5:.5e}\t{6:.5e}\n"
+        metricsStr = "".join(metricsTemplate.format(chrDict[locationArr[i, 0]], locationArr[i, 1:3],
+                                                    nameArr[maxDiffArr[i] - 1], abs(distanceArrReal[i]),
+                                                    findSign(distanceArrReal[i]), pvals[i], mhPvals[i])
+                             for i in range(len(distanceArrReal)))
+    else:
+        metricsTemplate = "{0}\t{1[0]}\t{1[1]}\t{2}\t{3:.5f}\t{4}\n"
+        metricsStr = "".join(metricsTemplate.format(chrDict[locationArr[i, 0]], locationArr[i, 1:3],
+                                                    nameArr[maxDiffArr[i] - 1], abs(distanceArrReal[i]),
+                                                    findSign(distanceArrReal[i]))
+                             for i in range(len(distanceArrReal)))
 
     metricsTxt.write(metricsStr)
     metricsTxt.close()
 
 
-def createTopScoresTxt(filePath, locationArr, chrDict, distanceArr, maxDiffArr, nameArr, pvals, onlySignificant, mhPvals):
+def createSignificantLociTxt(filePath, locationArr, chrDict, distanceArr, maxDiffArr, nameArr, pvals, mhPvals):
     """
-    Finds the either the 1000 largest distance bins and merges adjacent bins or finds all significant loci and does not merge.
-    Then it outputs a txt containing these highest distances regions and some information about each (chromosome, bin start,
-    bin end, state name, absolute value of distance, sign of score, pvalue of distance, stars repersenting significance)
+    Finds all significant loci and outputs a txt containing these highest distances regions and some information about
+    each (chromosome, bin start, bin end, state name, absolute value of distance, sign of distance, pvalue of distance,
+    stars repersenting significance)
 
     Input:
-    filePath -- The path of the file to write to
+    filePath    -- The path of the file to write to
     locationArr -- Numpy array containing the genomic locations of all the bins
-    chrDict -- Dictionary containing mappings between number values and chromosome names (helps locationArr use less memory)
+    chrDict     -- Dictionary containing mappings between number values and chromosome names (helps use less memory)
     distanceArr -- Numpy array containing the distance between the pairwise groups
-    maxDiffArr -- Numpy array containing the states which had the largest difference in each bin
-    nameArr -- Numpy array containing the names of all the states
-    pvals -- Numpy array containing the pvalues of all the distances between the pairwise groups
-    onlySignificant -- Boolean telling us whether to use significant loci or 1000 largest distance bins
-    mhPvals -- Multiple hypothesis corrected pvals using the Benjamini-Hochberg procedure
-    """
-    f = gzip.open(filePath, "wt") if onlySignificant else open(filePath, 'w')
-
-    # Pick values above significance threshold and then sort
-    indices = np.where(mhPvals <= 0.1)[0][(-np.abs(distanceArr[np.where(mhPvals <= 0.1)[0]])).argsort()]
-
-    # Make sure that there are at least 1000 values if creating greatestHits.txt
-    if not onlySignificant and len(indices) < 1000:
-        indices = (-np.abs(distanceArr)).argsort()[:1000]
-
-    locations = pd.DataFrame(np.concatenate((locationArr[indices], distanceArr[indices].reshape(len(indices), 1),
-                                             maxDiffArr[indices].reshape(len(indices), 1),
-                                             pvals[indices].reshape(len(indices), 1),
-                                             mhPvals[indices].reshape(len(indices), 1)), axis=1),
+    maxDiffArr  -- Numpy array containing the states which had the largest difference in each bin
+    nameArr     -- Numpy array containing the names of all the states
+    pvals       -- Numpy array containing the pvalues of all the distances between the pairwise groups
+    mhPvals     -- Multiple hypothesis corrected pvals using the Benjamini-Hochberg procedure
+
+    Output:
+    significantLoci*.txt.gz file which contains all loci found to be significantly different. Formatted as follows:
+        Column 1: Chromosome
+        Column 2: Start coordinate
+        Column 3: End coordinate
+        Column 4: Name of the largest difference state
+        Column 5: Squared euclidean distance between the scores
+        Column 6: Direction of the distance (sign determined by the higher signal between groups 1 and 2)
+        Column 7: P-Value of the distance
+        Column 8: Benjamini–Hochberg adjusted P-Value of the distance
+        Column 9: Stars indicating multiple hypothesis adjusted p-value of distance
+                  ('***' at .01, '**' at .05, and '*' at .1)
+    """
+    outfile = gzip.open(filePath, "wt")
+
+    # Pick values above significance threshold
+    indices = maxIndices = np.where(mhPvals <= 0.1)[0]
+
+    if len(indices) == 0:
+        outfile.close()
+        return
+
+    locations = pd.DataFrame(np.concatenate((locationArr[indices], distanceArr[maxIndices].reshape(len(maxIndices), 1),
+                                             maxDiffArr[maxIndices].reshape(len(maxIndices), 1),
+                                             pvals[maxIndices].reshape(len(maxIndices), 1),
+                                             mhPvals[maxIndices].reshape(len(maxIndices), 1)), axis=1),
                              columns=["Chromosome", "Start", "End", "Score", "MaxDiffLoc", "Pval", "MhPval"])\
-                  .astype({"Chromosome": np.int32, "Start": np.int32, "End": np.int32, "Score": np.float32,
+                  .astype({"Chromosome": np.int32, "Start": np.int64, "End": np.int64, "Score": np.float32,
                            "MaxDiffLoc": np.int32, "Pval": np.float32, "MhPval": np.float32})\
                   .replace({"Chromosome": chrDict})
 
-    # Don't want to merge when creating significantLoci.txt
-    if not onlySignificant:
-        locations = mergeAdjacent(pr.PyRanges(locations))
-        if "Start_b" in locations.columns:
-            locations.drop(columns=["Start_b", "End_b"], inplace=True)
-
-    # Sort by absolute value of score
-    locations = locations.iloc[(-locations["Score"].abs()).argsort()]
-
-    # Locations get 3 stars if they are significant at .01, 2 stars at .05, 1 star at .1, and a period if not significant
+    # Locations get 3 stars if they are significant at .01, 2 stars at .05, 1 star at .1, and a period if nonsignificant
     stars = np.array(["***" if float(locations.iloc[i, 6]) <= 0.01 else
                       ("**" if float(locations.iloc[i, 6]) <= 0.05 else
                       ("*" if float(locations.iloc[i, 6]) <= 0.1 else "."))
-                      for i in range(locations.shape[0])]).reshape(locations.shape[0], 1)
+                      for i in range(locations.shape[0])])
 
-    # Write all the locations to the file for significantLoci.txt
-    # Write only top 100 loci to file for greatestHits.txt
+    # Write the locations to significantLoci.txt
     outTemplate = "{0[0]}\t{0[1]}\t{0[2]}\t{1}\t{2:.5f}\t{3}\t{4:.5e}\t{5:.5e}\t{6}\n"
     outString = "".join(outTemplate.format(locations.iloc[i], nameArr[int(float(locations.iloc[i, 4])) - 1],
                                            abs(float(locations.iloc[i, 3])), findSign(float(locations.iloc[i, 3])),
-                                           float(locations.iloc[i, 5]), float(locations.iloc[i, 6]), stars[i, 0])
-                        for i in range(locations.shape[0] if onlySignificant else min((locations.shape[0], 100))))
-    f.write(outString)
-    f.close()
-
+                                           float(locations.iloc[i, 5]), float(locations.iloc[i, 6]), stars[i])
+                        for i in range(locations.shape[0]))
 
-def mergeAdjacent(originalLocations):
-    """
-    Takes a pyranges object and merges all adjacent regions maintaining the highest score
+    outfile.write(outString)
+    outfile.close()
 
-    Input:
-    originalLocations -- Pyranges object containing loci, scores, and more (not relevant for function)
 
-    Ouput:
-    pandas dataframe with adjacent regions merged
+def createROITxt(filePath, locationArr, chrDict, distanceArr, maxDiffArr, nameArr, pvals, mhPvals, roiWidth):
     """
-    mergedData = originalLocations.merge()
-    joinMergedToOriginal = mergedData.join(originalLocations)
+    Finds the top 100 regions of interest using filter-regions maxmean algorithm. Of these, those which have at least
+    one significantly different bin are output into a .txt file
 
-    # finalMerge is a pyranges object
-    finalMerge = joinMergedToOriginal.apply(maxScoringElement)
-    # finalMerge.df is a pandas dataframe
-    return finalMerge.df
+    Input:
+    filePath    -- The path of the file to write to
+    locationArr -- Numpy array containing the genomic locations of all the bins
+    chrDict     -- Dictionary containing mappings between number values and chromosome names (helps use less memory)
+    distanceArr -- Numpy array containing the distance between the pairwise groups
+    maxDiffArr  -- Numpy array containing the states which had the largest difference in each bin
+    nameArr     -- Numpy array containing the names of all the states
+    pvals       -- Numpy array containing the pvalues of all the distances between the pairwise groups
+    mhPvals     -- Multiple hypothesis corrected pvals using the Benjamini-Hochberg procedure
+    roiWidth    -- size of regions of interest in bins
 
+    Output:
+    regionsOfInterest*.txt file formatted as follows:
+        Column 1: Chromosome
+        Column 2: Start coordinate
+        Column 3: End coordinate
+        Column 4: Name of the largest difference state
+        Column 5: Squared euclidean distance between the scores
+        Column 6: Direction of the distance (sign determined by the higher signal between groups 1 and 2)
+        Column 7: P-Value of the distance
+        Column 8: Benjamini–Hochberg adjusted P-Value of the distance
+        Column 9: Stars indicating multiple hypothesis adjusted p-value of distance
+                  ('***' at .01, '**' at .05, and '*' at .1)
+    """
+    outfile = open(filePath, 'w')
+
+    # Using the filter-regions package for the meanmax algorithm to choose regions
+    rois, indices = maxMean(np.concatenate((locationArr, np.abs(distanceArr).reshape(len(distanceArr), 1)), axis=1),
+                            roiWidth, 100)
+
+    # Generating array of all indices for vectorized calculations
+    roiIndicesArr = generateROIIndicesArr(indices, roiWidth)
+
+    # Find the index of the maximally differential bin in the region
+    maxIndices = np.argmax(np.abs(distanceArr)[roiIndicesArr], axis=1) + roiIndicesArr[:, 0]
+
+    # in the case of creating regions of interest indices should be a intersection of all significantLoci and regions
+    # generated by maxmean because indices will be sorted by the max, we can cut off loci on the first instance where
+    # the max isn't significant
+    firstNonSigIdx = np.where(mhPvals[maxIndices] > 0.1)[0]
+    if len(firstNonSigIdx) > 0:
+        firstNonSigIdx = np.min(firstNonSigIdx)
+        maxIndices = maxIndices[:firstNonSigIdx]
+        rois = rois[:firstNonSigIdx]
+
+    if len(maxIndices) == 0:
+        outfile.close()
+        return
+
+    # Build the actual dataframe
+    locations = pd.DataFrame(rois.loc[:, ["Chromosome", "Start", "End"]])\
+                  .astype({"Chromosome": np.int32, "Start": np.int64, "End": np.int64})\
+                  .replace({"Chromosome": chrDict})
+    locations["Score"] = distanceArr[maxIndices].astype(np.float32)
+    locations["maxDiffLoc"] = maxDiffArr[maxIndices].astype(np.int32)
+    locations["Pval"] = pvals[maxIndices].astype(np.float32)
+    locations["MhPval"] = mhPvals[maxIndices].astype(np.float32)
 
-def maxScoringElement(df):
-    """
-    Takes a dataframe and deletes duplicate rows, maintaining the highest score
+    # Locations get 3 stars if they are significant at .01, 2 stars at .05, 1 star at .1, and a period if nonsignificant
+    stars = np.array(["***" if float(locations.iloc[i, 6]) <= 0.01 else
+                     ("**" if float(locations.iloc[i, 6]) <= 0.05 else
+                     ("*" if float(locations.iloc[i, 6]) <= 0.1 else "."))
+                     for i in range(locations.shape[0])])
 
-    Input:
-    df -- pandas dataframe containing merged loci
+    # Write only top 100 loci to file for regionsOfInterest*.txt
+    outTemplate = "{0[0]}\t{0[1]}\t{0[2]}\t{1}\t{2:.5f}\t{3}\t{4:.5e}\t{5:.5e}\t{6}\n"
+    outString = "".join(outTemplate.format(locations.iloc[i], nameArr[int(float(locations.iloc[i, 4])) - 1],
+                                           abs(float(locations.iloc[i, 3])), findSign(float(locations.iloc[i, 3])),
+                                           float(locations.iloc[i, 5]), float(locations.iloc[i, 6]), stars[i])
+                        for i in range(locations.shape[0]))
 
-    Output:
-    pandas dataframe with deleted duplicate rows
-    """
-    return df.iloc[(-df["Score"].abs()).argsort()].drop_duplicates(['Chromosome', 'Start', 'End'], keep='first')
+    outfile.write(outString)
+    outfile.close()
 
 
-def findSign(x):
+def createROINoSignificance(filePath, locationArr, chrDict, distanceArr, maxDiffArr, nameArr, zScores, roiWidth):
     """
-    Returns a string containing the sign of the inputted number
+    Finds the top 100 regions of interest using filter-regions maxmean algorithm and outputs them in a txt file
 
     Input:
-    x -- Any number
+    filePath    -- The path of the file to write to
+    locationArr -- Numpy array containing the genomic locations of all the bins
+    chrDict     -- Dictionary containing mappings between number values and chromosome names (helps use less memory)
+    distanceArr -- Numpy array containing the distance between the pairwise groups
+    maxDiffArr  -- Numpy array containing the states which had the largest difference in each bin
+    nameArr     -- Numpy array containing the names of all the states
+    zScores     -- Absolute value of the ZScores of the distances
+    roiWidth    -- size of regions of interest in bins
 
     Output:
-    "+" or "-"
-    """
-    if (x >= 0):
-        return "+"
-    else:
-        return "-"
+    regionsOfInterest*.txt file formatted as follows
+        Column 1: Chromosome
+        Column 2: Start coordinate
+        Column 3: End coordinate
+        Column 4: Name of the largest difference state
+        Column 5: Squared euclidean distance between the scores
+        Column 6: Direction of the distance (sign determined by the higher signal between groups 1 and 2)
+        Column 7: Z-score of the distance
+        Column 8: Stars indicating Z-score of distance ('***' stars at >=3, '**' at >=2, '*' at >=1, '.' if <1)
+    """
+    outfile = open(filePath, 'w')
+
+    # Using the filter-regions package for the meanmax algorithm to choose regions
+    rois, indices = maxMean(np.concatenate((locationArr, np.abs(distanceArr).reshape(len(distanceArr), 1)), axis=1),
+                            roiWidth, 100)
+
+    # Generating array of all indices for vectorized calculations
+    roiIndicesArr = generateROIIndicesArr(indices, roiWidth)
+
+    # Find the index of the maximally differential bin in the region
+    maxIndices = np.argmax(np.abs(distanceArr)[roiIndicesArr], axis=1) + roiIndicesArr[:, 0]
+
+    # Build the actual dataframe
+    locations = pd.DataFrame(rois.loc[:, ["Chromosome", "Start", "End"]])\
+                  .astype({"Chromosome": np.int32, "Start": np.int64, "End": np.int64})\
+                  .replace({"Chromosome": chrDict})
+    locations["Score"] = distanceArr[maxIndices].astype(np.float32)
+    locations["maxDiffLoc"] = maxDiffArr[maxIndices].astype(np.int32)
+    locations["ZScores"] = zScores[maxIndices].astype(np.float32)
+
+    # Locations get 3 stars if they are 3 sd away, 2 at 2 sd, 1 at 1 sd, and a period if withing 1 sd
+    stars = np.array(["***" if float(locations.iloc[i, 5]) >= 3 else
+                      ("**" if float(locations.iloc[i, 5]) >= 2 else
+                      ("*" if float(locations.iloc[i, 5]) >= 1 else "."))
+                      for i in range(locations.shape[0])])
+
+    # Write only top 100 loci to file for regionsOfInterest.txt
+    outTemplate = "{0[0]}\t{0[1]}\t{0[2]}\t{1}\t{2:.5f}\t{3}\t{4:.5f}\t{5}\n"
+    outString = "".join(outTemplate.format(locations.iloc[i], nameArr[int(float(locations.iloc[i, 4])) - 1],
+                                           abs(float(locations.iloc[i, 3])), findSign(float(locations.iloc[i, 3])),
+                                           float(locations.iloc[i, 5]), stars[i])
+                        for i in range(len(indices)))
+
+    outfile.write(outString)
+    outfile.close()
 
 
-def createGenomeManhattan(group1Name, group2Name, locationArr, chrDict, distanceArrReal, maxDiffArr, beta, loc, scale,
-                          stateColorList, outputDirPath, fileTag, mhPvals):
+def createGenomeManhattan(group1Name, group2Name, locationArr, chrDict, distanceArrReal, maxDiffArr, stateColorList,
+                          outputDirPath, fileTag, pvalBool, beta=0, loc=0, scale=0, mhPvals=[], zScores=[]):
     """
     Creates a manhattan plot based on the distances between the two groups for the entire genome
 
     Input:
-    group1Name -- The name of the first epilogos group
-    group2Name -- The name of the second epilogos group
-    locationArr -- Numpy array containing the genomic locations of all the bins
-    chrDict -- Dictionary containing mappings between number values and chromosome names (helps locationArr use less memory)
+    group1Name      -- The name of the first epilogos group
+    group2Name      -- The name of the second epilogos group
+    locationArr     -- Numpy array containing the genomic locations of all the bins
+    chrDict         -- Dictionary containing mappings between number values and chromosome names (helps use less memory)
     distanceArrReal -- Numpy array containing the real distances
-    maxDiffArr -- Numpy array containing the states which had the largest difference between the two groups in each bin
-    beta -- gennorm fit parameter
-    loc -- gennorm fit parameter
-    scale -- gennorm fit parameter
-    stateColorList -- Numpy array containing the colors of each of the states in the state model
-    outputDirPath -- The path of the output directory for epilogos
-    fileTag -- A string which helps ensure outputed files are named similarly within an epilogos run
-    mhPvals -- Multiple hypothesis corrected pvals using the Benjamini-Hochberg procedure
+    maxDiffArr      -- Numpy array containing the states which had the largest difference between the two groups in
+                       each bin
+    stateColorList  -- Numpy array containing the colors of each of the states in the state model
+    outputDirPath   -- The path of the output directory for epilogos
+    fileTag         -- A string which helps ensure outputed files are named similarly within an epilogos run
+    pvalBool        -- A boolean telling us whether we are using pvals or not
+    beta            -- gennorm fit parameter
+    loc             -- gennorm fit parameter
+    scale           -- gennorm fit parameter
+    mhPvals         -- Multiple hypothesis corrected pvals using the Benjamini-Hochberg procedure
+    zScores         -- Absolute value of the Z-Scores of the scores in the case that we are not using pvals
+
+    Output:
+    Genome wide manhattan plot depiciting the per bin distances between the two sample groups
     """
     manhattanDirPath = outputDirPath / "manhattanPlots_{}".format(fileTag)
     if not manhattanDirPath.exists():
         manhattanDirPath.mkdir(parents=True)
 
     fig = plt.figure(figsize=(16, 9))
     ax = fig.add_subplot(111)
@@ -662,190 +817,218 @@
     ax.spines["top"].set_visible(False)
     ax.spines["right"].set_visible(False)
     ax.spines["bottom"].set_visible(False)
     plt.title("Differential epilogos between {} and {} biosamples".format(group1Name, group2Name))
     ax.set_ylabel("Distance")
     plt.xlabel("Chromosome")
     xticks = np.where(locationArr[:, 1] == 0)[0]
-    plt.xticks(ticks=xticks, labels=list(map(lambda x: x.split("chr")[-1], [chrDict[x] for x in locationArr[:, 0][xticks]])))
+    plt.xticks(ticks=xticks, labels=list(map(lambda x: x.split("chr")[-1],
+                                             [chrDict[x] for x in locationArr[:, 0][xticks]])))
 
     plt.margins(x=0)
     ylim = np.amax(np.abs(distanceArrReal)) * 1.1
     ax.set_ylim(-ylim, ylim)
-    yticks, ytickLabels = pvalAxisScaling(ylim, beta, loc, scale)
+    yticks, ytickLabels = pvalAxisScaling(ylim, beta, loc, scale) if pvalBool \
+        else zScoreAxisScaling(ylim, np.mean(distanceArrReal), np.std(distanceArrReal))
 
     ax.set_yticks(yticks)
     ax.set_yticklabels([str(np.abs(np.round(val, 1))) for val in yticks])
 
     axR = ax.twinx()
-    axR.set_ylabel("P-Value")
+    axR.set_ylabel("P-Value" if pvalBool else "Z-Score")
     axR.spines["top"].set_visible(False)
     axR.spines["left"].set_visible(False)
     axR.spines["bottom"].set_visible(False)
     axR.set_yticks(yticks)
     axR.set_ylim(ax.get_ylim())
     axR.set_yticklabels(ytickLabels)
 
-    ax.text(0.99, 0.99, group1Name, verticalalignment='top', horizontalalignment='right', transform=ax.transAxes, fontsize=15)
+    ax.text(0.99, 0.99, group1Name, verticalalignment='top', horizontalalignment='right', transform=ax.transAxes,
+            fontsize=15)
     ax.text(0.99, 0.01, group2Name, verticalalignment='bottom', horizontalalignment='right', transform=ax.transAxes,
             fontsize=15)
 
     locationOnGenome = np.arange(len(distanceArrReal))
 
     for i in range(len(xticks)):
-        if i == len(xticks)-1:
-            points = np.where((locationOnGenome >= xticks[i]) & (mhPvals > 0.1))[0]
+        if i == len(xticks) - 1:
+            points = np.where((locationOnGenome >= xticks[i]) & (mhPvals > 0.1))[0] if pvalBool\
+                else np.where((locationOnGenome >= xticks[i]) & (zScores < 10))[0]
+            color = "gray" if i % 2 == 0 else "black"
             plt.scatter(locationOnGenome[points], distanceArrReal[points],
-                        s=(np.abs(distanceArrReal[points]) / np.amax(np.abs(distanceArrReal)) * 100), color="gray",
+                        s=(np.abs(distanceArrReal[points]) / np.amax(np.abs(distanceArrReal)) * 100), color=color,
                         marker=".", alpha=0.1, edgecolors='none', rasterized=True)
         elif i % 2 == 0:
-            points = np.where((locationOnGenome >= xticks[i]) & (locationOnGenome < xticks[i+1])
-                              & (mhPvals > 0.1))[0]
+            if pvalBool:
+                points = np.where((locationOnGenome >= xticks[i]) & (locationOnGenome < xticks[i + 1])
+                                  & (mhPvals > 0.1))[0]
+            else:
+                points = np.where((locationOnGenome >= xticks[i]) & (locationOnGenome < xticks[i + 1])
+                                  & (zScores < 10))[0]
             plt.scatter(locationOnGenome[points], distanceArrReal[points],
                         s=(np.abs(distanceArrReal[points]) / np.amax(np.abs(distanceArrReal)) * 100), color="gray",
                         marker=".", alpha=0.1, edgecolors='none', rasterized=True)
         else:
-            points = np.where((locationOnGenome >= xticks[i]) & (locationOnGenome < xticks[i+1])
-                              & (mhPvals > 0.1))[0]
+            if pvalBool:
+                points = np.where((locationOnGenome >= xticks[i]) & (locationOnGenome < xticks[i + 1])
+                                  & (mhPvals > 0.1))[0]
+            else:
+                points = np.where((locationOnGenome >= xticks[i]) & (locationOnGenome < xticks[i + 1])
+                                  & (zScores < 10))[0]
             plt.scatter(locationOnGenome[points], distanceArrReal[points],
                         s=(np.abs(distanceArrReal[points]) / np.amax(np.abs(distanceArrReal)) * 100), color="black",
                         marker=".", alpha=0.1, edgecolors='none', rasterized=True)
 
-    point1Indices  = np.where(mhPvals <= 0.1)[0]
-    point05Indices = np.where(mhPvals <= 0.05)[0]
-    point01Indices = np.where(mhPvals <= 0.01)[0]
-
-    colorArr = stateColorList[maxDiffArr[point1Indices].astype(int) - 1]
-    opacityArr = np.array((np.abs(distanceArrReal[point1Indices]) /
-                           np.amax(np.abs(distanceArrReal)))).reshape(len(distanceArrReal[point1Indices]), 1)
+    line1Indices = np.where(mhPvals <= 0.1)[0] if pvalBool else np.where(zScores >= 10)[0]
+    line2Indices = np.where(mhPvals <= 0.05)[0] if pvalBool else np.where(zScores >= 20)[0]
+    line3Indices = np.where(mhPvals <= 0.01)[0] if pvalBool else np.where(zScores >= 30)[0]
+
+    colorArr = stateColorList[maxDiffArr[line1Indices].astype(int) - 1]
+    opacityArr = np.array((np.abs(distanceArrReal[line1Indices])
+                           / np.amax(np.abs(distanceArrReal)))).reshape(len(distanceArrReal[line1Indices]), 1)
     rgbaColorArr = np.concatenate((colorArr, opacityArr), axis=1)
-    sizeArr = np.abs(distanceArrReal[point1Indices]) / np.amax(np.abs(distanceArrReal)) * 100
+    sizeArr = np.abs(distanceArrReal[line1Indices]) / np.amax(np.abs(distanceArrReal)) * 100
 
-    plt.scatter(point1Indices, distanceArrReal[point1Indices], s=sizeArr, color=rgbaColorArr, marker=".",
+    plt.scatter(line1Indices, distanceArrReal[line1Indices], s=sizeArr, color=rgbaColorArr, marker=".",
                 edgecolors='none', rasterized=True)
 
-    if len(point01Indices) > 0:
-        point1Line = np.min(np.abs(distanceArrReal[point1Indices]))
-        point05Line = np.min(np.abs(distanceArrReal[point05Indices]))
-        point01Line = np.min(np.abs(distanceArrReal[point01Indices]))
+    if len(line3Indices) > 0:
+        point1Line = np.min(np.abs(distanceArrReal[line1Indices]))
+        point05Line = np.min(np.abs(distanceArrReal[line2Indices]))
+        point01Line = np.min(np.abs(distanceArrReal[line3Indices]))
         plt.axhspan(point1Line, point05Line, facecolor='black', alpha=0.05)
         plt.axhspan(point05Line, point01Line, facecolor='black', alpha=0.10)
         plt.axhspan(point01Line, ylim, facecolor='black', alpha=0.15)
         plt.axhspan(-point1Line, -point05Line, facecolor='black', alpha=0.05)
         plt.axhspan(-point05Line, -point01Line, facecolor='black', alpha=0.10)
         plt.axhspan(-point01Line, -ylim, facecolor='black', alpha=0.15)
-    elif len(point05Indices) > 0:
-        point1Line = np.min(np.abs(distanceArrReal[point1Indices]))
-        point05Line = np.min(np.abs(distanceArrReal[point05Indices]))
+    elif len(line2Indices) > 0:
+        point1Line = np.min(np.abs(distanceArrReal[line1Indices]))
+        point05Line = np.min(np.abs(distanceArrReal[line2Indices]))
         plt.axhspan(point1Line, point05Line, facecolor='black', alpha=0.05)
         plt.axhspan(point05Line, ylim, facecolor='black', alpha=0.10)
         plt.axhspan(-point1Line, -point05Line, facecolor='black', alpha=0.05)
         plt.axhspan(-point05Line, -ylim, facecolor='black', alpha=0.10)
-    elif len(point1Indices) > 0:
-        point1Line = np.min(np.abs(distanceArrReal[point1Indices]))
+    elif len(line1Indices) > 0:
+        point1Line = np.min(np.abs(distanceArrReal[line1Indices]))
         plt.axhspan(point1Line, ylim, facecolor='black', alpha=0.05)
         plt.axhspan(-point1Line, -ylim, facecolor='black', alpha=0.05)
 
     figPath = manhattanDirPath / "manhattan_plot_genome.pdf"
     fig.savefig(figPath, bbox_inches='tight', dpi=400, facecolor="#FFFFFF", edgecolor="#FFFFFF", transparent=False)
     fig.clear()
     plt.close(fig)
 
 
 def _initChromosomeManhattan(group1Name_, group2Name_, locationArr_, distanceArrReal_, maxDiffArr_, params, mhPvals_,
-                             stateColorList_, manhattanDirPath_):
+                             zScores_, stateColorList_, manhattanDirPath_, pvalBool_):
     """
     Initializes global variables for multiprocessing in the single epilogos case
 
     Input:
-    group1Name_ -- The name of the first epilogos group
-    group2Name_ -- The name of the second epilogos group
-    locationArr_ -- Numpy array containing the genomic locations of all the bins
-    distanceArrReal_ -- Numpy array containing the real distances
-    maxDiffArr_ -- Numpy array containing the states which had the largest difference between the two groups in each bin
-    params -- gennorm fit parameters
-    mhPvals_ -- Multiple hypothesis corrected pvals using the Benjamini-Hochberg procedure
-    stateColorList_ -- Numpy array containing the colors of each of the states in the state model
+    group1Name_       -- The name of the first epilogos group
+    group2Name_       -- The name of the second epilogos group
+    locationArr_      -- Numpy array containing the genomic locations of all the bins
+    distanceArrReal_  -- Numpy array containing the real distances
+    maxDiffArr_       -- Numpy array containing the states which had the largest difference between the two groups in
+                         each bin
+    params            -- gennorm fit parameters
+    mhPvals_          -- Multiple hypothesis corrected pvals using the Benjamini-Hochberg procedure
+    zScores_          -- Absolute values of the z-scores of the distances
+    stateColorList_   -- Numpy array containing the colors of each of the states in the state model
     manhattanDirPath_ -- The path to directory to put manhattan plots
+    pvalBool_         -- A boolean to tell us whether we will use pvals or zscores
     """
     global group1Name
     global group2Name
     global locationArr
     global distanceArrReal
     global maxDiffArr
     global beta
     global loc
     global scale
     global mhPvals
+    global zScores
     global stateColorList
     global manhattanDirPath
+    global pvalBool
 
     group1Name = group1Name_
     group2Name = group2Name_
     locationArr = locationArr_
     distanceArrReal = distanceArrReal_
     maxDiffArr = maxDiffArr_
     beta, loc, scale = params[:-2], params[-2], params[-1]
     mhPvals = mhPvals_
+    zScores = zScores_
     stateColorList = stateColorList_
     manhattanDirPath = manhattanDirPath_
+    pvalBool = pvalBool_
 
 
-def createChromosomeManhattan(group1Name, group2Name, locationArr, chrDict, distanceArrReal, maxDiffArr, params,
-                              stateColorList, outputDirPath, fileTag, numProcesses, mhPvals):
+def createChromosomeManhattan(group1Name, group2Name, locationArr, chrDict, distanceArrReal, maxDiffArr, stateColorList,
+                              outputDirPath, fileTag, numProcesses, pvalBool, params=[0, 0, 0], mhPvals=[], zScores=[]):
     """
     Creates a manhattan plot based on the distances between the two groups for the each chromosome
 
     Input:
-    group1Name -- The name of the first epilogos group
-    group2Name -- The name of the second epilogos group
-    locationArr -- Numpy array containing the genomic locations of all the bins
-    chrDict -- Dictionary containing mappings between number values and chromosome names (helps locationArr use less memory)
+    group1Name      -- The name of the first epilogos group
+    group2Name      -- The name of the second epilogos group
+    locationArr     -- Numpy array containing the genomic locations of all the bins
+    chrDict         -- Dictionary containing mappings between number values and chromosome names (helps use less memory)
     distanceArrReal -- Numpy array containing the real distances
-    maxDiffArr -- Numpy array containing the states which had the largest difference between the two groups in each bin
-    params -- gennorm fit parameters
-    stateColorList -- Numpy array containing the colors of each of the states in the state model
-    outputDirPath -- The path of the output directory for epilogos
-    fileTag -- A string which helps ensure outputed files are named similarly within an epilogos run
-    numProcesses -- The number of cores to run on
-    mhPvals -- Multiple hypothesis corrected pvals using the Benjamini-Hochberg procedure
+    maxDiffArr      -- Numpy array containing the states which had the largest difference between the two groups in
+                       each bin
+    stateColorList  -- Numpy array containing the colors of each of the states in the state model
+    outputDirPath   -- The path of the output directory for epilogos
+    fileTag         -- A string which helps ensure outputed files are named similarly within an epilogos run
+    numProcesses    -- The number of cores to run on
+    pvalBool        -- A boolean value to tell us whether we are going to use pvals or not
+    params          -- gennorm fit parameters
+    mhPvals         -- Multiple hypothesis corrected pvals using the Benjamini-Hochberg procedure
+    zScores         -- Absolute values of the Z-Scores of the distances
+
+    Output:
+    A chromosome wide manhattan plot depicting the per bin distances between groups for each chromosome
     """
     manhattanDirPath = outputDirPath / "manhattanPlots_{}".format(fileTag)
     if not manhattanDirPath.exists():
         manhattanDirPath.mkdir(parents=True)
 
     xticks = np.where(locationArr[:, 1] == 0)[0]
     startEnd = []
     for i in range(len(xticks)):
         if not i == len(xticks) - 1:
-            startEnd.append((xticks[i], xticks[i+1]))
+            startEnd.append((xticks[i], xticks[i + 1]))
         else:
             startEnd.append((xticks[i], -1))
 
     chrOrder = list(map(lambda x: x.split("chr")[-1], [chrDict[x] for x in locationArr[:, 0][xticks]]))
 
     # Multiprocess the reading
-    with closing(Pool(numProcesses, initializer=_initChromosomeManhattan, initargs=(group1Name, group2Name, locationArr,
-                                                                                    distanceArrReal, maxDiffArr, params,
-                                                                                    mhPvals, stateColorList,
-                                                                                    manhattanDirPath))) as pool:
+    with closing(Pool(numProcesses, initializer=_initChromosomeManhattan,
+                      initargs=(group1Name, group2Name, locationArr, distanceArrReal, maxDiffArr, params, mhPvals,
+                                zScores, stateColorList, manhattanDirPath, pvalBool))) as pool:
         pool.starmap(graphChromosomeManhattan, zip(chrOrder, startEnd))
     pool.join()
 
 
 def graphChromosomeManhattan(chromosome, startEnd):
     """
     Generates the manhattan plots for each chromosome based on the distances between the two groups.
     Note there are global variables which are used across all chromosomes (see _init())
 
     Input:
     chromosome -- The chromosome which we are plotting
-    startEnd -- The start and end indices for the chromosome on all the global numpy arrays
+    startEnd   -- The start and end indices for the chromosome on all the global numpy arrays
 
     Also see global variables from _initChromosomeManhattan above
+
+    Output:
+    A chromosome wide manhattan plot depicting the per bin distances between groups for the specified chromosome
     """
     fig = plt.figure(figsize=(16, 9))
     ax = fig.add_subplot(111)
     ax.set_facecolor("#FFFFFF")
     ax.set_axisbelow(True)
     ax.grid(True, axis='y', color='k', linewidth=.25, linestyle="-")
     ax.spines["top"].set_visible(False)
@@ -855,128 +1038,173 @@
     plt.xlabel("Location in Chromosome {} (Mb)".format(chromosome))
     plt.title("Differential epilogos between {} and {} donor biosamples (Chromosome {})".format(group1Name, group2Name,
                                                                                                 chromosome))
 
     plt.margins(x=0)
     ylim = np.amax(np.abs(distanceArrReal)) * 1.1
     ax.set_ylim(-ylim, ylim)
-    yticks, ytickLabels = pvalAxisScaling(ylim, beta, loc, scale)
+    yticks, ytickLabels = pvalAxisScaling(ylim, beta, loc, scale) if pvalBool\
+        else zScoreAxisScaling(ylim, np.mean(distanceArrReal), np.std(distanceArrReal))
 
     ax.set_yticks(yticks)
     ax.set_yticklabels([str(np.abs(np.round(val, 1))) for val in yticks])
 
     axR = ax.twinx()
-    axR.set_ylabel("P-Value")
+    axR.set_ylabel("P-Value" if pvalBool else "Z-Score")
     axR.spines["top"].set_visible(False)
     axR.spines["left"].set_visible(False)
     axR.spines["bottom"].set_visible(False)
     axR.set_yticks(yticks)
     axR.set_ylim(ax.get_ylim())
     axR.set_yticklabels(ytickLabels)
 
-    ax.text(0.99, 0.99, group1Name, verticalalignment='top', horizontalalignment='right', transform=ax.transAxes, fontsize=15)
+    ax.text(0.99, 0.99, group1Name, verticalalignment='top', horizontalalignment='right', transform=ax.transAxes,
+            fontsize=15)
     ax.text(0.99, 0.01, group2Name, verticalalignment='bottom', horizontalalignment='right', transform=ax.transAxes,
             fontsize=15)
 
     locationOnGenome = np.arange(len(distanceArrReal))
 
     if startEnd[1] == -1:
         realxticks = np.where((locationOnGenome >= startEnd[0]) & (locationArr[:, 1].astype(int) % 10000000 == 0))[0]
-        plt.xticks(ticks=realxticks, labels=[str(int(int(locationArr[tick, 1])/1000000)) for tick in realxticks])
+        plt.xticks(ticks=realxticks, labels=[str(int(int(locationArr[tick, 1]) / 1000000)) for tick in realxticks])
 
-        points = np.where((locationOnGenome >= startEnd[0]) & (mhPvals > 0.1))[0]
+        points = np.where((locationOnGenome >= startEnd[0]) & (mhPvals > 0.1))[0] if pvalBool\
+            else np.where((locationOnGenome >= startEnd[0]) & (zScores < 10))[0]
         plt.scatter(locationOnGenome[points], distanceArrReal[points],
-                    s=(np.abs(distanceArrReal[points]) / np.amax(np.abs(distanceArrReal)) * 100), color="gray", marker=".",
-                    alpha=0.1, edgecolors='none', rasterized=True)
+                    s=(np.abs(distanceArrReal[points]) / np.amax(np.abs(distanceArrReal)) * 100), color="gray",
+                    marker=".", alpha=0.1, edgecolors='none', rasterized=True)
 
-        point1Indices  = np.where((locationOnGenome >= startEnd[0]) & (mhPvals <= 0.1))[0]
-        point05Indices = np.where((locationOnGenome >= startEnd[0]) & (mhPvals <= 0.05))[0]
-        point01Indices = np.where((locationOnGenome >= startEnd[0]) & (mhPvals <= 0.01))[0]
+        line1Indices = np.where((locationOnGenome >= startEnd[0]) & (mhPvals <= 0.1))[0] if pvalBool\
+            else np.where((locationOnGenome >= startEnd[0]) & (zScores >= 10))[0]
+        line2Indices = np.where((locationOnGenome >= startEnd[0]) & (mhPvals <= 0.05))[0] if pvalBool\
+            else np.where((locationOnGenome >= startEnd[0]) & (zScores >= 20))[0]
+        line3Indices = np.where((locationOnGenome >= startEnd[0]) & (mhPvals <= 0.01))[0] if pvalBool\
+            else np.where((locationOnGenome >= startEnd[0]) & (zScores >= 30))[0]
 
     else:
         realxticks = np.where(((locationOnGenome >= startEnd[0]) & (locationOnGenome < startEnd[1]))
                               & (locationArr[:, 1].astype(int) % 10000000 == 0))[0]
-        plt.xticks(ticks=realxticks, labels=[str(int(int(locationArr[tick, 1])/1000000)) for tick in realxticks])
+        plt.xticks(ticks=realxticks, labels=[str(int(int(locationArr[tick, 1]) / 1000000)) for tick in realxticks])
 
-        points = np.where(((locationOnGenome >= startEnd[0]) & (locationOnGenome < startEnd[1]))
-                          & (mhPvals > 0.1))[0]
+        if pvalBool:
+            points = np.where(((locationOnGenome >= startEnd[0]) & (locationOnGenome < startEnd[1]))
+                              & (mhPvals > 0.1))[0]
+        else:
+            points = np.where(((locationOnGenome >= startEnd[0]) & (locationOnGenome < startEnd[1]))
+                              & (zScores < 10))[0]
         plt.scatter(locationOnGenome[points], distanceArrReal[points],
-                    s=(np.abs(distanceArrReal[points]) / np.amax(np.abs(distanceArrReal)) * 100), color="gray", marker=".",
-                    alpha=0.1, edgecolors='none', rasterized=True)
+                    s=(np.abs(distanceArrReal[points]) / np.amax(np.abs(distanceArrReal)) * 100), color="gray",
+                    marker=".", alpha=0.1, edgecolors='none', rasterized=True)
 
-        point1Indices  = np.where(((locationOnGenome >= startEnd[0]) & (locationOnGenome <= startEnd[1]))
-                                  & (mhPvals <= 0.1))[0]
-        point05Indices = np.where(((locationOnGenome >= startEnd[0]) & (locationOnGenome <= startEnd[1]))
-                                  & (mhPvals <= 0.05))[0]
-        point01Indices = np.where(((locationOnGenome >= startEnd[0]) & (locationOnGenome <= startEnd[1]))
-                                  & (mhPvals <= 0.01))[0]
-
-    colorArr = stateColorList[maxDiffArr[point1Indices].astype(int) - 1]
-    opacityArr = np.array((np.abs(distanceArrReal[point1Indices]) /
-                           np.amax(np.abs(distanceArrReal)))).reshape(len(distanceArrReal[point1Indices]), 1)
+        if pvalBool:
+            line1Indices = np.where(((locationOnGenome >= startEnd[0]) & (locationOnGenome <= startEnd[1]))
+                                    & (mhPvals <= 0.1))[0]
+            line2Indices = np.where(((locationOnGenome >= startEnd[0]) & (locationOnGenome <= startEnd[1]))
+                                    & (mhPvals <= 0.05))[0]
+            line3Indices = np.where(((locationOnGenome >= startEnd[0]) & (locationOnGenome <= startEnd[1]))
+                                    & (mhPvals <= 0.01))[0]
+        else:
+            line1Indices = np.where(((locationOnGenome >= startEnd[0]) & (locationOnGenome <= startEnd[1]))
+                                    & (zScores >= 10))[0]
+            line2Indices = np.where(((locationOnGenome >= startEnd[0]) & (locationOnGenome <= startEnd[1]))
+                                    & (zScores >= 20))[0]
+            line3Indices = np.where(((locationOnGenome >= startEnd[0]) & (locationOnGenome <= startEnd[1]))
+                                    & (zScores >= 30))[0]
+
+    colorArr = stateColorList[maxDiffArr[line1Indices].astype(int) - 1]
+    opacityArr = np.array((np.abs(distanceArrReal[line1Indices])
+                           / np.amax(np.abs(distanceArrReal)))).reshape(len(distanceArrReal[line1Indices]), 1)
     rgbaColorArr = np.concatenate((colorArr, opacityArr), axis=1)
-    sizeArr = np.abs(distanceArrReal[point1Indices]) / np.amax(np.abs(distanceArrReal)) * 100
+    sizeArr = np.abs(distanceArrReal[line1Indices]) / np.amax(np.abs(distanceArrReal)) * 100
 
-    plt.scatter(point1Indices, distanceArrReal[point1Indices], s=sizeArr, color=rgbaColorArr, marker=".",
+    plt.scatter(line1Indices, distanceArrReal[line1Indices], s=sizeArr, color=rgbaColorArr, marker=".",
                 edgecolors='none', rasterized=True)
 
-    if len(point01Indices) > 0:
-        point1Line = np.min(np.abs(distanceArrReal[point1Indices]))
-        point05Line = np.min(np.abs(distanceArrReal[point05Indices]))
-        point01Line = np.min(np.abs(distanceArrReal[point01Indices]))
+    if len(line3Indices) > 0:
+        point1Line = np.min(np.abs(distanceArrReal[line1Indices]))
+        point05Line = np.min(np.abs(distanceArrReal[line2Indices]))
+        point01Line = np.min(np.abs(distanceArrReal[line3Indices]))
         plt.axhspan(point1Line, point05Line, facecolor='black', alpha=0.05)
         plt.axhspan(point05Line, point01Line, facecolor='black', alpha=0.10)
         plt.axhspan(point01Line, ylim, facecolor='black', alpha=0.15)
         plt.axhspan(-point1Line, -point05Line, facecolor='black', alpha=0.05)
         plt.axhspan(-point05Line, -point01Line, facecolor='black', alpha=0.10)
         plt.axhspan(-point01Line, -ylim, facecolor='black', alpha=0.15)
-    elif len(point05Indices) > 0:
-        point1Line = np.min(np.abs(distanceArrReal[point1Indices]))
-        point05Line = np.min(np.abs(distanceArrReal[point05Indices]))
+    elif len(line2Indices) > 0:
+        point1Line = np.min(np.abs(distanceArrReal[line1Indices]))
+        point05Line = np.min(np.abs(distanceArrReal[line2Indices]))
         plt.axhspan(point1Line, point05Line, facecolor='black', alpha=0.05)
         plt.axhspan(point05Line, ylim, facecolor='black', alpha=0.10)
         plt.axhspan(-point1Line, -point05Line, facecolor='black', alpha=0.05)
         plt.axhspan(-point05Line, -ylim, facecolor='black', alpha=0.10)
-    elif len(point1Indices) > 0:
-        point1Line = np.min(np.abs(distanceArrReal[point1Indices]))
+    elif len(line1Indices) > 0:
+        point1Line = np.min(np.abs(distanceArrReal[line1Indices]))
         plt.axhspan(point1Line, ylim, facecolor='black', alpha=0.05)
         plt.axhspan(-point1Line, -ylim, facecolor='black', alpha=0.05)
 
     figPath = manhattanDirPath / "manhattan_plot_chr{}.pdf".format(chromosome)
     fig.savefig(figPath, bbox_inches='tight', dpi=400, facecolor="#FFFFFF", edgecolor="#FFFFFF", transparent=False)
     fig.clear()
     plt.close(fig)
 
 
 def pvalAxisScaling(ylim, beta, loc, scale):
     """
     Generates list containing proper tick marks for the manhattan plots
 
     Input:
-    ylim -- The y limit of the manhattan plot
-    beta -- gennorm fit parameter
-    loc -- gennorm fit parameter
+    ylim  -- The y limit of the manhattan plot
+    beta  -- gennorm fit parameter
+    loc   -- gennorm fit parameter
     scale -- gennorm fit parameter
+
+    Output:
+    (yticksFinal, ytickLabelsFinal) -- The y-tick axis labels for all p-values within the y-axis range
     """
     yticks = []
     ytickLabels = ["$10^{%d}$" % i for i in range(-16, -3)] + ["$1$"] + ["$10^{-%d}$" % i for i in range(4, 17)]
 
     for i in range(-16, -3):
-        yticks.append(-st.gennorm.isf(10**i/2, beta, loc=loc, scale=scale))
-        yticks.append(st.gennorm.isf(10**i/2, beta, loc=loc, scale=scale))
+        yticks.append(-st.gennorm.isf(10 ** i / 2, beta, loc=loc, scale=scale))
+        yticks.append(st.gennorm.isf(10 ** i / 2, beta, loc=loc, scale=scale))
     yticks.append(0)
     yticks.sort()
 
     yticksFinal = []
     ytickLabelsFinal = []
 
     for i in range(len(yticks)):
         if yticks[i] >= -ylim and yticks[i] <= ylim:
             yticksFinal.append(float(yticks[i]))
             ytickLabelsFinal.append(ytickLabels[i])
 
     return (yticksFinal, ytickLabelsFinal)
 
 
+def zScoreAxisScaling(ylim, mean, stanDev):
+    """
+    Generates list containing proper tick marks for the manhattan plots according to z-score
+
+    Input:
+    ylim    -- The y limit of the manhattan plot
+    mean    -- the mean of the scores
+    stanDev -- the standard deviation of the scores
+
+    Output:
+    (yticks, ytickLabels) -- The y-tick axis labels for all zscores within the y-axis range
+    """
+
+    maxZScore = (ylim - mean) / stanDev
+
+    yticks = []
+    ytickLabels = ["{0:.1f}".format(i) for i in np.linspace(-maxZScore, maxZScore, 11)]
+
+    for i in np.linspace(-maxZScore, maxZScore, 11):
+        yticks.append(round(i, 1) * stanDev + mean)
+
+    return (yticks, ytickLabels)
+
+
 if __name__ == "__main__":
-    main(argv[1], argv[2], argv[3], argv[4], argv[5], int(argv[6]), strToBool(argv[7]), int(argv[8]), int(argv[9]), argv[10],
-         strToBool(argv[11]))
+    main(argv[1], argv[2], argv[3], argv[4], argv[5], int(argv[6]), strToBool(argv[7]), strToBool(argv[8]),
+         int(argv[9]), int(argv[10]), argv[11], int(argv[12]), strToBool(argv[13]))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `epilogos-0.1.1/epilogos/run.py` & `epilogos-0.1.2/epilogos/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,59 +6,78 @@
 from pathlib import PurePath
 import errno
 import click
 
 from epilogos.expected import main as expected
 from epilogos.expectedCombination import main as expectedCombination
 from epilogos.scores import main as scores
-from epilogos.greatestHits import main as greatestHits
-from epilogos.pairwiseVisual import main as pairwiseVisual
+from epilogos.roiSingle import main as roiSingle
+from epilogos.roiAndVisualPairwise import main as roiPairwise
 from epilogos.helpers import getNumStates
 
 
 @click.command(context_settings=dict(help_option_names=['-h', '--help']))
-@click.option("-m", "--mode", "mode", type=click.Choice(["single", "paired"]), default=["single"], show_default=True,
-              multiple=True, help="single for single group epilogos and paired for 2 group epilogos")
-@click.option("-l", "--local", "commandLineBool", is_flag=True, multiple=True,
+@click.option("-m", "--mode", "mode", type=click.Choice(["single", "paired"]), default="single", show_default=True,
+              help="single for single group epilogos and paired for 2 group epilogos")
+@click.option("-l", "--local", "commandLineBool", is_flag=True,
               help="If enabled, Epilogos will run locally in your terminal rather than on a SLURM cluster")
-@click.option("-i", "--input-directory", "inputDirectory", type=str, multiple=True,
+@click.option("-i", "--input-directory", "inputDirectory", type=str,
               help="Path to directory that contains files to read from (ALL files in this directory will be read in)")
-@click.option("-a", "--directory-one", "inputDirectory1", type=str, multiple=True,
-              help="Path to first directory that contains files to read from (ALL files in this directory will be read in)")
-@click.option("-b", "--directory-two", "inputDirectory2", type=str, multiple=True,
-              help="Path to second directory that contains files to read from (ALL files in this directory will be read in)")
-@click.option("-o", "--output-directory", "outputDirectory", type=str, multiple=True,
+@click.option("-a", "--directory-one", "inputDirectory1", type=str,
+              help="Path to first directory that contains files to read from "
+                   + "(ALL files in this directory will be read in)")
+@click.option("-b", "--directory-two", "inputDirectory2", type=str,
+              help="Path to second directory that contains files to read from "
+                   + "(ALL files in this directory will be read in)")
+@click.option("-o", "--output-directory", "outputDirectory", type=str,
               help="Output Directory (CANNOT be the same as input directory)\n")
-@click.option("-n", "--state-info", "stateInfo", type=str, multiple=True, help="State model info file")
-@click.option("-s", "--saliency", "saliency", type=int, default=[1], show_default=True, multiple=True,
+@click.option("-j", "--state-info", "stateInfo", type=str, help="State model info file")
+@click.option("-s", "--saliency", "saliency", type=int, default=1, show_default=True,
               help="Desired saliency level (1, 2, or 3)")
-@click.option("-c", "--num-cores", "numProcesses", type=int, default=[0], multiple=True,
-              help="The number of cores to run on [default: 0 = Uses all cores]")
-@click.option("-x", "--exit", "exitBool", is_flag=True, multiple=True,
-              help="If flag is enabled program will exit upon submission of all SLURM processes rather than completion of " +
-                   "all processes")
-@click.option("-d", "--diagnostic-figures", "diagnosticBool", is_flag=True, multiple=True,
-              help="If flag is enabled, program will output some diagnostic figures of the gennorm fit on the null data and " +
-                   "comparisons between the null and real data")
-@click.option("-t", "--num-trials", "numTrials", type=int, default=[101], show_default=True, multiple=True,
-              help="The number of times subsamples of the scores are fit")
-@click.option("-z", "--sampling-size", "samplingSize", type=int, default=[100000], show_default=True, multiple=True,
-              help="The size of the subsamples on which the scores are fit")
-@click.option("-q", "--quiescent-state", "quiescentState", type=int, multiple=True,
-              help="If a bin contains only states of this value, it is treated as quiescent and not factored into fitting." +
-                   "If set to 0, filtering is not done. [default: last state]")
-@click.option("-g", "--group-size", "groupSize", type=int, default=[-1], show_default=True, multiple=True,
-              help="In pairwise epilogos controls the sizes of the shuffled arrays. Default is sizes of the input groups")
-@click.option("-v", "--version", "version", is_flag=True, multiple=True,
+@click.option("-c", "--num-cores", "numProcesses", type=int, default=1,
+              help="The number of cores to run on (0=Uses all cores) [default: 1]")
+@click.option("-x", "--exit", "exitBool", is_flag=True,
+              help="If flag is enabled program will exit upon submission of all SLURM processes rather than "
+                   + "completion of all processes")
+@click.option("-d", "--diagnostic-figures", "diagnosticBool", is_flag=True,
+              help="If flag is enabled, program will output some diagnostic figures of the gennorm fit on the null "
+                   + "data and comparisons between the null and real data")
+@click.option("-t", "--num-trials", "numTrials", type=int, default=101, show_default=True,
+              help="The number of times subsamples of the scores are fit when using a null distribution")
+@click.option("-z", "--sampling-size", "samplingSize", type=int, default=100000, show_default=True,
+              help="The size of the subsamples on which the scores are fit when using a null distribution")
+@click.option("-q", "--quiescent-state", "quiescentState", type=int, default=-1,
+              help="If a bin contains only states of this value, it is treated as quiescent and not factored into "
+                   + "fitting. If set to 0, filtering is not done. [default: last state]")
+@click.option("-g", "--group-size", "groupSize", type=int, default=-1, show_default=True,
+              help="In pairwise epilogos controls the sizes of the shuffled arrays. "
+                   + "Default is sizes of the input groups")
+@click.option("-v", "--version", "version", is_flag=True,
               help="If flag is enabled epilogos will print the installed version number and exit")
-@click.option("-p", "--partition", "partition", type=str, multiple=True,
-              help="Request a specific partition for the SLURM resource allocation. If not specified, uses the default " +
-                   "partition as designated by the system administrator")
+@click.option("-p", "--partition", "partition", type=str,
+              help="Request a specific partition for the SLURM resource allocation. If not specified, uses the "
+                   + "default partition as designated by the system administrator")
+@click.option("-n", "--null-distribution", "pvalBool", is_flag=True,
+              help="If flag is enabled, epilogos will calculate p-values for pairwise scores")
+@click.option("-w", "--roi-width", "roiWidth", type=int, default=0,
+              help="The number of bins in a region of interest [default: 50(single)/125(paired)]")
+@click.option("-f", "--file-tag", "fileTag", type=str, default="null",
+              help="Tag to be appended in output filenames [default: input-directory_saliency]")
+@click.option("--exp-freq-mem", "expFreqMem", type=int, default=20000,
+              help="Memory (in MB) for the expected frequency calcuation jobs [default: 20000]")
+@click.option("--exp-comb-mem", "expCombMem", type=int, default=8000,
+              help="Memory (in MB) for the expected frequency combination job [default: 8000]")
+@click.option("--score-mem", "scoreMem", type=int, default=40000,
+              help="Memory (in MB) for the expected frequency calcuation jobs [default: 40000]")
+@click.option("--roi-mem", "roiMem", type=int, default=-1,
+              help="Memory (in MB) for the expected frequency calcuation jobs "
+                   + "[default: 20000 (single) / 100000 (paired)]")
 def main(mode, commandLineBool, inputDirectory, inputDirectory1, inputDirectory2, outputDirectory, stateInfo, saliency,
-         numProcesses, exitBool, diagnosticBool, numTrials, samplingSize, quiescentState, groupSize, version, partition):
+         numProcesses, exitBool, diagnosticBool, numTrials, samplingSize, quiescentState, groupSize, version, partition,
+         pvalBool, roiWidth, fileTag, expFreqMem, expCombMem, scoreMem, roiMem):
     """
     Information-theoretic navigation of multi-tissue functional genomic annotations
 
     Written by Jacob Quon and Wouter Meuleman
     """
 
     print("""\n
@@ -81,47 +100,44 @@
 
     if version:
         from epilogos import __version__
         print("Version:", __version__)
         sys.exit()
 
     # Make sure all flags are submitted as expected
-    checkFlags(mode, commandLineBool, inputDirectory, inputDirectory1, inputDirectory2, outputDirectory, stateInfo, saliency,
-               numProcesses, exitBool, diagnosticBool, numTrials, samplingSize, quiescentState, groupSize, partition)
+    checkFlags(mode, commandLineBool, inputDirectory, inputDirectory1, inputDirectory2, outputDirectory, stateInfo,
+               exitBool, diagnosticBool, partition, pvalBool)
 
-    # Pull info out of the flags
-    mode, outputDirectory, stateInfo, saliency, numProcesses, numTrials, samplingSize, groupSize = \
-        mode[0], outputDirectory[0], stateInfo[0], saliency[0], numProcesses[0], numTrials[0], samplingSize[0], groupSize[0]
-    diagnosticBool = True if diagnosticBool else False
     verbose = False if commandLineBool else True
     numStates = getNumStates(stateInfo)
     # Quiescent value is user input - 1 because states are read in to be -1 from their values
-    quiescentState = quiescentState[0] - 1 if quiescentState else numStates - 1
+    quiescentState = numStates - 1 if quiescentState == -1 else quiescentState - 1
+
+    # setting roiWidth from default of 0
+    if roiWidth == 0:
+        roiWidth = 50 if mode == "single" else 125
 
     # Get paths from arguments and turn them into absolute paths
     if mode == "single":
-        inputDirectory = inputDirectory[0]
         inputDirPath = Path(inputDirectory)
         inputDirPath2 = ""
     else:
-        inputDirectory = inputDirectory1[0]
-        inputDirectory2 = inputDirectory2[0]
-        inputDirPath = Path(inputDirectory)
+        inputDirPath = Path(inputDirectory1)
         inputDirPath2 = Path(inputDirectory2)
         if not PurePath(inputDirPath2).is_absolute():
             inputDirPath2 = Path.cwd() / inputDirPath2
     if not PurePath(inputDirPath).is_absolute():
         inputDirPath = Path.cwd() / inputDirPath
     outputDirPath = Path(outputDirectory)
     if not PurePath(outputDirPath).is_absolute():
         outputDirPath = Path.cwd() / outputDirPath
 
     # Make sure argments are valid
-    checkArguments(mode, saliency, inputDirPath, inputDirPath2, outputDirPath, numProcesses, numStates, quiescentState,
-                   groupSize)
+    checkArguments(mode, saliency, inputDirPath, inputDirPath2, outputDirPath, numProcesses, numStates, numTrials,
+                   samplingSize, quiescentState, groupSize, roiWidth)
 
     # Informing user of their inputs
     print()
     if mode == "single":
         print("Input Directory =", inputDirPath)
     else:
         print("Input Directory 1 =", inputDirPath)
@@ -129,40 +145,36 @@
     print("State Model =", numStates)
     print("Saliency level =", saliency)
     print("Output Directory =", outputDirPath)
     if numProcesses == 0:
         print("Number of Cores = All available", flush=True)
     else:
         print("Number of Cores =", numProcesses, flush=True)
-    if mode == "paired" and quiescentState == -1:
+    if mode == "paired" and quiescentState == -1:  # If quiescentState was user input as 0 it is now -1
         print("Quiescent State = No quiescent filtering")
     elif mode == "paired":
         print("Quiescent State =", quiescentState + 1)
 
     # For making sure all files are consistently named
-    if mode == "single":
-        fileTag = "{}_s{}".format(inputDirPath.name, saliency)
-    else:
-        fileTag = "{}_{}_s{}".format(inputDirPath.name, inputDirPath2.name, saliency)
+    if fileTag == "null":
+        if mode == "single":
+            fileTag = "{}_s{}".format(inputDirPath.name, saliency)
+        else:
+            fileTag = "{}_{}_s{}".format(inputDirPath.name, inputDirPath2.name, saliency)
 
     # Path for storing/retrieving the expected frequency array
     storedExpPath = outputDirPath / "exp_freq_{}.npy".format(fileTag)
 
     if not commandLineBool:
         # Variable for the sbatch submission in case we are using slurm
-        if numProcesses == 0:
-            memory = "--exclusive --mem=0"
-        else:
-            memory = "--ntasks={} --mem=16000".format(numProcesses)
-
-            print("\nWARNING: {} cores requested.".format(numProcesses), flush=True, end=" ")
-            print("Machine specs unknown, requesting 16gb of memory across all cores")
+        expFreqMem, expCombMem, scoreMem, roiMem = determineMemories(numProcesses, expFreqMem, expCombMem, scoreMem,
+                                                                     roiMem, mode)
 
         if partition:
-            partition = "--partition=" + partition[0]
+            partition = "--partition=" + partition
         else:
             partition = ""
 
         # Creating directories for slurm output and error logs
         (outputDirPath / ".out/").mkdir(parents=True, exist_ok=True)
         (outputDirPath / ".err/").mkdir(parents=True, exist_ok=True)
         print("\nSlurm .out log files are located at: {}".format(outputDirPath / ".out/"))
@@ -177,316 +189,286 @@
 
     # Calculate the expected frequency for each file in the input directory
     expJobIDArr = []
     print("\nSTEP 1: Per data file background frequency calculation", flush=True)
     for file in inputDirPath.glob("*"):
         if mode == "single":
             if commandLineBool:
-                # epilogos.expected.expected(file, "null", numStates, saliency, outputDirPath, fileTag, numProcesses, verbose)
                 expected(file, "null", numStates, saliency, outputDirPath, fileTag, numProcesses, verbose)
             else:
                 computeExpectedPy = pythonFilesDir / "expected.py"
-                pythonCommand = "python {} {} null {} {} {} {} {} {}".format(computeExpectedPy, file, numStates, saliency,
-                                                                             outputDirPath, fileTag, numProcesses, verbose)
+                pythonCommand = "python {} {} null {} {} {} {} {} {}".format(computeExpectedPy, file, numStates,
+                                                                             saliency, outputDirPath, fileTag,
+                                                                             numProcesses, verbose)
                 expJobIDArr.append(submitSlurmJob("_" + file.name.split(".")[0], "exp_calc", fileTag, outputDirPath,
-                                                  pythonCommand, saliency, partition, memory, ""))
+                                                  pythonCommand, saliency, partition, expFreqMem, ""))
         else:
             # Find matching file in other directory
             if not list(inputDirPath2.glob(file.name)):
-                raise FileNotFoundError("File not found: {}".format(str(inputDirPath2 / file.name)) +
-                                        "Please ensure corresponding files within input directories directories 1 and 2 have" +
-                                        " the same name")
+                raise FileNotFoundError("File not found: {}".format(str(inputDirPath2 / file.name))
+                                        + "Please ensure corresponding files within input directories "
+                                        + "directories 1 and 2 have the same name")
             else:
                 file2 = next(inputDirPath2.glob(file.name))
 
             if commandLineBool:
-                # epilogos.expected.expected(file, file2, numStates, saliency, outputDirPath, fileTag, numProcesses, verbose)
                 expected(file, file2, numStates, saliency, outputDirPath, fileTag, numProcesses, verbose)
             else:
                 computeExpectedPy = pythonFilesDir / "expected.py"
                 pythonCommand = "python {} {} {} {} {} {} {} {} {}".format(computeExpectedPy, file, file2, numStates,
-                                                                           saliency, outputDirPath, fileTag, numProcesses,
-                                                                           verbose)
+                                                                           saliency, outputDirPath, fileTag,
+                                                                           numProcesses, verbose)
                 expJobIDArr.append(submitSlurmJob("_" + file.name.split(".")[0], "exp_calc", fileTag, outputDirPath,
-                                                  pythonCommand, saliency, partition, memory, ""))
+                                                  pythonCommand, saliency, partition, expFreqMem, ""))
 
     if not commandLineBool:
         # Create a string for slurm dependency to work and to print more nicely
         expJobIDStr = str(expJobIDArr).strip('[]').replace(" ", "")
         print("    JobIDs:", expJobIDStr, flush=True)
 
     # Combining all the different chromosome expected frequency arrays into one
     print("\nSTEP 2: Background frequency combination", flush=True)
     if commandLineBool:
         expectedCombination(outputDirPath, storedExpPath, fileTag, verbose)
     else:
         computeExpectedCombinationPy = pythonFilesDir / "expectedCombination.py"
-        pythonCommand = "python {} {} {} {} {}".format(computeExpectedCombinationPy, outputDirPath, storedExpPath, fileTag,
-                                                       verbose)
+        pythonCommand = "python {} {} {} {} {}".format(computeExpectedCombinationPy, outputDirPath, storedExpPath,
+                                                       fileTag, verbose)
         combinationJobID = submitSlurmJob("", "exp_comb", fileTag, outputDirPath, pythonCommand, saliency, partition,
-                                          "--ntasks=1 --mem=8000", "--dependency=afterok:{}".format(expJobIDStr))
+                                          expCombMem, "--dependency=afterok:{}".format(expJobIDStr))
         print("    JobID:", combinationJobID, flush=True)
 
     scoreJobIDArr = []
     # Calculate the observed frequencies and scores
     print("\nSTEP 3: Score calculation", flush=True)
     for file in inputDirPath.glob("*"):
         if mode == "single":
             if commandLineBool:
                 scores(file, "null", numStates, saliency, outputDirPath, storedExpPath, fileTag, numProcesses,
                        quiescentState, groupSize, verbose)
             else:
                 computeScorePy = pythonFilesDir / "scores.py"
                 pythonCommand = "python {} {} null {} {} {} {} {} {} {} {} {}".format(computeScorePy, file, numStates,
-                                                                                      saliency, outputDirPath, storedExpPath,
-                                                                                      fileTag, numProcesses, quiescentState,
+                                                                                      saliency, outputDirPath,
+                                                                                      storedExpPath, fileTag,
+                                                                                      numProcesses, quiescentState,
                                                                                       groupSize, verbose)
                 scoreJobIDArr.append(submitSlurmJob("_" + file.name.split(".")[0], "score", fileTag, outputDirPath,
-                                                    pythonCommand, saliency, partition, memory,
+                                                    pythonCommand, saliency, partition, scoreMem,
                                                     "--dependency=afterok:{}".format(combinationJobID)))
         else:
             # Find matching file in other directory
             if not list(inputDirPath2.glob(file.name)):
-                raise FileNotFoundError("File not found: {}".format(str(inputDirPath2 / file.name)) +
-                                        "Please ensure corresponding files within input directories directories 1 and 2 have" +
-                                        " the same name")
+                raise FileNotFoundError("File not found: {}".format(str(inputDirPath2 / file.name))
+                                        + "Please ensure corresponding files within input directories "
+                                        + "directories 1 and 2 have the same name")
             else:
                 file2 = next(inputDirPath2.glob(file.name))
 
             if commandLineBool:
                 scores(file, file2, numStates, saliency, outputDirPath, storedExpPath, fileTag, numProcesses,
                        quiescentState, groupSize, verbose)
             else:
                 computeScorePy = pythonFilesDir / "scores.py"
-                pythonCommand = "python {} {} {} {} {} {} {} {} {} {} {} {}".format(computeScorePy, file, file2, numStates,
-                                                                                    saliency, outputDirPath, storedExpPath,
-                                                                                    fileTag, numProcesses, quiescentState,
+                pythonCommand = "python {} {} {} {} {} {} {} {} {} {} {} {}".format(computeScorePy, file, file2,
+                                                                                    numStates, saliency, outputDirPath,
+                                                                                    storedExpPath, fileTag,
+                                                                                    numProcesses, quiescentState,
                                                                                     groupSize, verbose)
                 scoreJobIDArr.append(submitSlurmJob("_" + file.name.split(".")[0], "score", fileTag, outputDirPath,
-                                                    pythonCommand, saliency, partition, memory,
+                                                    pythonCommand, saliency, partition, scoreMem,
                                                     "--dependency=afterok:{}".format(combinationJobID)))
 
     if not commandLineBool:
         # Create a string for slurm dependency to work
         scoreJobIDStr = str(scoreJobIDArr).strip('[]').replace(" ", "")
         print("    JobIDs:", scoreJobIDStr, flush=True)
 
     if mode == "single":
-        # Create a greatest hits text file
-        print("\nSTEP 4: Finding greatest hits", flush=True)
+        # Create a regions of interest text file
+        print("\nSTEP 4: Finding regions of interest", flush=True)
         if commandLineBool:
-            greatestHits(outputDirPath, stateInfo, fileTag, storedExpPath, verbose)
+            roiSingle(outputDirPath, stateInfo, fileTag, storedExpPath, roiWidth, verbose)
         else:
-            computeGreatestHitsPy = pythonFilesDir / "greatestHits.py"
-            pythonCommand = "python {} {} {} {} {} {}".format(computeGreatestHitsPy, outputDirPath, stateInfo, fileTag,
-                                                              storedExpPath, verbose)
-            summaryJobID = submitSlurmJob("", "hits", fileTag, outputDirPath, pythonCommand, saliency, partition,
-                                          "--ntasks=1 --mem=16000", "--dependency=afterok:{}".format(scoreJobIDStr))
+            computeROISinglePy = pythonFilesDir / "roiSingle.py"
+            pythonCommand = "python {} {} {} {} {} {} {}".format(computeROISinglePy, outputDirPath, stateInfo, fileTag,
+                                                                 storedExpPath, roiWidth, verbose)
+            summaryJobID = submitSlurmJob("", "roi", fileTag, outputDirPath, pythonCommand, saliency, partition,
+                                          roiMem, "--dependency=afterok:{}".format(scoreJobIDStr))
             print("    JobID:", summaryJobID, flush=True)
     else:
         # Fitting, calculating p-values, and visualizing pairiwse differences
-        print("\nSTEP 4: Generating p-values and figures", flush=True)
+        print("\nSTEP 4: Generating p-values, rois, & figures", flush=True)
         if commandLineBool:
-            pairwiseVisual(inputDirPath.name, inputDirPath2.name, stateInfo, outputDirPath, fileTag, numProcesses,
-                           diagnosticBool, numTrials, samplingSize, storedExpPath, verbose)
+            roiPairwise(inputDirPath.name, inputDirPath2.name, stateInfo, outputDirPath, fileTag, numProcesses,
+                        pvalBool, diagnosticBool, numTrials, samplingSize, storedExpPath, roiWidth, verbose)
         else:
-            computeVisualPy = pythonFilesDir / "pairwiseVisual.py"
-            pythonCommand = "python {} {} {} {} {} {} {} {} {} {} {} {}".format(computeVisualPy, inputDirPath.name,
-                                                                                inputDirPath2.name, stateInfo, outputDirPath,
-                                                                                fileTag, numProcesses, diagnosticBool,
-                                                                                numTrials, samplingSize, storedExpPath,
-                                                                                verbose)
-            summaryJobID = submitSlurmJob("", "visual", fileTag, outputDirPath, pythonCommand, saliency, partition, memory,
-                                          "--dependency=afterok:{}".format(scoreJobIDStr))
+            computeROIPairwisePy = pythonFilesDir / "roiAndVisualPairwise.py"
+            pythonCommand = "python {} {} {} {} {} {} {} {} {} {} {} {} {} {}".format(computeROIPairwisePy,
+                                                                                      inputDirPath.name,
+                                                                                      inputDirPath2.name, stateInfo,
+                                                                                      outputDirPath, fileTag,
+                                                                                      numProcesses, pvalBool,
+                                                                                      diagnosticBool, numTrials,
+                                                                                      samplingSize, storedExpPath,
+                                                                                      roiWidth, verbose)
+            summaryJobID = submitSlurmJob("", "visual", fileTag, outputDirPath, pythonCommand, saliency, partition,
+                                          roiMem, "--dependency=afterok:{}".format(scoreJobIDStr))
             print("    JobID:", summaryJobID, flush=True)
 
     if not commandLineBool:
         allJobIDs = "{},{},{},{}".format(expJobIDStr, combinationJobID, scoreJobIDStr, summaryJobID)
         print("\nAll JobIDs:\n    ", allJobIDs, flush=True)
 
     # If the user wants to exit upon job completion rather than submission
     # If a job fails, it cancels all other jobs
     if not commandLineBool and not exitBool:
         checkExit(mode, allJobIDs, expJobIDArr, scoreJobIDArr, outputDirPath, saliency)
 
 
-def checkFlags(mode, commandLineBool, inputDirectory, inputDirectory1, inputDirectory2, outputDirectory, stateInfo, saliency,
-               numProcesses, exitBool, diagnosticBool, numTrials, samplingSize, quiescentState, groupSize, partition):
+def checkFlags(mode, commandLineBool, inputDirectory, inputDirectory1, inputDirectory2, outputDirectory, stateInfo,
+               exitBool, diagnosticBool, partition, pvalBool):
     """
-    Checks all the input flags are makes sure that there are not duplicates, required flags are present, and incompatible flags
-    are not present together
+    Checks all the input flags are makes sure that there are not duplicates, required flags are present, and
+    incompatible flags are not present together
 
     Input:
     See click options at top of script
     """
     # Checking that all required flags are inputted
-    if mode[0] == "single" and not inputDirectory:
+    if mode == "single" and not inputDirectory:
         print("ERROR: [-i, --input-directory] required in 'single' group mode")
         sys.exit()
-    elif mode[0] == "paired" and not inputDirectory1:
+    elif mode == "paired" and not inputDirectory1:
         print("ERROR: [-a, --directory-one] required in 'paired' group mode")
         sys.exit()
-    elif mode[0] == "paired" and not inputDirectory2:
+    elif mode == "paired" and not inputDirectory2:
         print("ERROR: [-b, --directory-two] required in 'paired' group mode")
         sys.exit()
     elif not outputDirectory:
         print("ERROR: [-o, --output-directory] required")
         sys.exit()
     elif not stateInfo:
         print("ERROR: [-n, --state-info] required")
         sys.exit()
 
     # Checking that incompatible flags are not input together
-    if mode[0] == "single" and inputDirectory1:
+    if mode == "single" and inputDirectory1:
         print("ERROR: [-m, --mode] 'single' not compatible with [-a, --directory-one] option")
         sys.exit()
-    elif mode[0] == "single" and inputDirectory2:
+    elif mode == "single" and inputDirectory2:
         print("ERROR: [-m, --mode] 'single' not compatible with [-b, --directory-two] option")
         sys.exit()
-    elif mode[0] == "single" and diagnosticBool:
+    elif mode == "single" and diagnosticBool:
         print("ERROR: [-m, --mode] 'single' not compatible with [-d, --diagnostic-figures] flag")
         sys.exit()
-    elif mode[0] == "single" and quiescentState:
-        print("ERROR: [-m, --mode] 'single' not compatible with [-q, --quiescent-state] flag")
+    elif mode == "single" and pvalBool:
+        print("ERROR: [-m, --mode] 'single' not compatible with [-n, --null-distribution] flag")
         sys.exit()
-    elif mode[0] == "paired" and inputDirectory:
+    elif mode == "paired" and inputDirectory:
         print("ERROR: [-m, --mode] 'paired' not compatible with [-i, --input-directory] option")
         sys.exit()
     elif commandLineBool and exitBool:
         print("ERROR: [-l, --cli] flag not compatible with [-x, --exit] flag")
         sys.exit()
     elif commandLineBool and partition:
         print("Error: [-l, --cli] flag not compatible with [-p, --partition] option")
         sys.exit()
 
-    # Checking if user inputs flag multiples times
-    if len(mode) > 1:
-        print("ERROR: Too many [-m, --mode] arguments provided")
-        sys.exit()
-    elif len(commandLineBool) > 1:
-        print("ERROR: Too many [-l, --cli] arguments provided")
-        sys.exit()
-    elif len(inputDirectory) > 1:
-        print("ERROR: Too many [-i, --input-directory] arguments provided")
-        sys.exit()
-    elif len(inputDirectory1) > 1:
-        print("ERROR: Too many [-a, --directory-one] arguments provided")
-        sys.exit()
-    elif len(inputDirectory2) > 1:
-        print("ERROR: Too many [-b, --directory-two] arguments provided")
-        sys.exit()
-    elif len(outputDirectory) > 1:
-        print("ERROR: Too many [-o, --output-directory] arguments provided")
-        sys.exit()
-    elif len(stateInfo) > 1:
-        print("ERROR: Too many [-n, --state-info] arguments provided")
-        sys.exit()
-    elif len(saliency) > 1:
-        print("ERROR: Too many [-s, --saliency] arguments provided")
-        sys.exit()
-    elif len(numProcesses) > 1:
-        print("ERROR: Too many [-c, --num-cores] arguments provided")
-        sys.exit()
-    elif len(exitBool) > 1:
-        print("ERROR: Too many [-x, --exit] arguments provided")
-        sys.exit()
-    elif len(diagnosticBool) > 1:
-        print("ERROR: Too many [-d, --diagnostic-figures] arguments provided")
-        sys.exit()
-    elif len(numTrials) > 1:
-        print("ERROR: Too many [-t, --num-trials] arguments provided")
-        sys.exit()
-    elif len(samplingSize) > 1:
-        print("ERROR: Too many [-z, --sampling-size] arguments provided")
-        sys.exit()
-    elif len(quiescentState) > 1:
-        print("ERROR: Too many [-q, --quiescent-state] arguments provided")
-        sys.exit()
-    elif len(groupSize) > 1:
-        print("ERROR: Too many [-g, --group-size] arguments provided")
-        sys.exit()
-    elif len(partition) > 1:
-        print("ERROR: Too many [-p, --partition] arguments provided")
-        sys.exit()
-
 
-def checkArguments(mode, saliency, inputDirPath, inputDirPath2, outputDirPath, numProcesses, numStates, quiescentState,
-                   groupSize):
+def checkArguments(mode, saliency, inputDirPath, inputDirPath2, outputDirPath, numProcesses, numStates, numTrials,
+                   samplingSize, quiescentState, groupSize, roiWidth):
     """
     Checks whether user submitted arguments have valid values
 
     Input:
-    mode -- 'single' or 'paired'; tells us which version of epilogos we are running
-    saliency -- The saliency metric input by the user
-    inputDirPath -- The path to the only input directory in single epilogos and the first input directory in paired epilogos
-    inputDirPath2 -- The path to the second input directory in the paired epilogos case
-    outputDirPath -- The path to the output directory for epilogos
-    numProcesses -- The number of cores the user would like to use
-    numStates -- The number of states in the state model
+    mode           -- 'single' or 'paired'; tells us which version of epilogos we are running
+    saliency       -- The saliency metric input by the user
+    inputDirPath   -- The path to the only input directory in single epilogos and the first input directory in paired
+                      epilogos
+    inputDirPath2  -- The path to the second input directory in the paired epilogos case
+    outputDirPath  -- The path to the output directory for epilogos
+    numProcesses   -- The number of cores the user would like to use
+    numStates      -- The number of states in the state model
+    numTrials      -- The number of gennorm fits to do in pairwise mode
+    samplingSize   -- The amount of null data to fit in pairwise mode
     quiescentState -- The state used to filter out quiescent bins
-    groupSize -- The size of the null (shuffled) score arrays, -1 means inputed sizes
+    groupSize      -- The size of the null (shuffled) score arrays, -1 means inputed sizes
+    roiWidth       -- size of regions of interest in bins
     """
     # Check validity of saliency
     if mode == "single" and saliency != 1 and saliency != 2 and saliency != 3:
-        print("ERROR: Saliency Metric Invalid: {}".format(saliency) +
-              "Please ensure that saliency metric is either 1, 2, or 3")
-        sys.exit()
+        raise ValueError("Saliency Metric Invalid: {}".format(saliency)
+                         + "Please ensure that saliency metric is either 1, 2, or 3")
     elif mode == "paired" and saliency != 1 and saliency != 2:
-        print("ERROR: Saliency Metric Invalid: {}".format(saliency) +
-              "Please ensure that saliency metric is either 1 or 2 (Saliency of 3 is unsupported for pairwise comparison")
-        sys.exit()
+        raise ValueError("Saliency Metric Invalid: {}".format(saliency)
+                         + "Please ensure that saliency metric is either 1 or 2 "
+                         + "(Saliency of 3 is unsupported for pairwise comparison")
 
     # Check validity of directories
     if not inputDirPath.exists():
         raise FileNotFoundError("Given path does not exist: {}".format(str(inputDirPath)))
     if not inputDirPath.is_dir():
         raise NotADirectoryError("Given path is not a directory: {}".format(str(inputDirPath)))
     if not list(inputDirPath.glob("*")):
-        raise OSError(errno.ENOTEMPTY, "Ensure given directory is not empty:", str(inputDirPath))
+        raise OSError(errno.ENOTEMPTY, "Ensure given directory is not empty", str(inputDirPath))
     if mode == "paired":
         if not inputDirPath2.exists():
             raise FileNotFoundError("Given path does not exist: {}".format(str(inputDirPath2)))
         if not inputDirPath2.is_dir():
             raise NotADirectoryError("Given path is not a directory: {}".format(str(inputDirPath2)))
         if not list(inputDirPath2.glob("*")):
-            raise OSError(errno.ENOTEMPTY, "Ensure given directory is not empty:", str(inputDirPath2))
+            raise OSError(errno.ENOTEMPTY, "Ensure given directory is not empty", str(inputDirPath2))
     if not outputDirPath.exists():
         outputDirPath.mkdir(parents=True)
     if not outputDirPath.is_dir():
         raise NotADirectoryError("Given path is not a directory: {}".format(str(outputDirPath)))
 
     if numProcesses < 0:
         print("ERROR: Number of cores must be positive or zero (0 means use all cores)")
         sys.exit()
 
+    if numTrials <= 0:
+        print("ERROR: Number of trials must be greater than zero")
+        sys.exit()
+
+    if samplingSize <= 0:
+        print("ERROR: Sampling size must be greater than zero")
+        sys.exit()
+
     if quiescentState < -1:
         print("ERROR: Quiescent state value must be positive or zero (0 means do not filter)")
         sys.exit()
     elif quiescentState >= numStates:
         print("ERROR: Quiescent state value must be a state provided in the state model")
         sys.exit()
 
     if groupSize < -1:
         print("ERROR: Group size value must be positive or -1 (-1 means use inputted group sizes)")
         sys.exit()
 
+    if roiWidth < 0:
+        print("ERROR: Group size value must be greater than 0")
+        sys.exit()
+
 
 def submitSlurmJob(filename, jobPrefix, fileTag, outputDirPath, pythonCommand, saliency, partition, memory, dependency):
     """
     Submits a epilogos job to a SLURM cluster
 
     Input:
-    filename -- The name of the file epilogos is using
-    jobPrefix -- The step of epilogos we are on ('exp_calc', 'exp_comb', 'score', 'visual', 'hits')
-    fileTag -- String that helps us ensure jobs are named consistenly across one epilogos run
+    filename      -- The name of the file epilogos is using
+    jobPrefix     -- The step of epilogos we are on ('exp_calc', 'exp_comb', 'score', 'visual', 'roi')
+    fileTag       -- String that helps us ensure jobs are named consistenly across one epilogos run
     outputDirPath -- The output directory for epilogos will be used for error and output logs
     pythonCommand -- The python command to run on the SLURM job
-    saliency -- The saliency metric being used in this epilogos run
-    memory -- The amount of memory to be allocated to the slurm job
-    dependency -- Which jobs the SLURM job must wait for before starting
+    saliency      -- The saliency metric being used in this epilogos run
+    paritition    -- The slurm paritition to use if user elected to choose a specific one
+    memory        -- The amount of memory to be allocated to the slurm job
+    dependency    -- Which jobs the SLURM job must wait for before starting
 
     Output:
     The job number
     """
     jobName = "{}_{}{}".format(jobPrefix, fileTag, filename)
     jobOutPath = outputDirPath / (".out/" + jobName + ".out")
     jobErrPath = outputDirPath / (".err/" + jobName + ".err")
@@ -524,20 +506,20 @@
 
 
 def checkExit(mode, allJobIDs, expJobIDArr, scoreJobIDArr, outputDirPath, saliency):
     """
     Prevents exiting of the main script until there is an error in one of the SLURM jobs or all SLURM jobs have finished
 
     Input:
-    mode -- 'single' or 'paired' depending on which version of epilogos we are running
-    allJobIDs -- String of all the SLURM job IDs
-    expJobIDArr -- List of the SLURM job IDs for the expected frequency step
+    mode          -- 'single' or 'paired' depending on which version of epilogos we are running
+    allJobIDs     -- String of all the SLURM job IDs
+    expJobIDArr   -- List of the SLURM job IDs for the expected frequency step
     scoreJobIDArr -- List of the SLURM job IDs for the score calculation step
     outputDirPath -- Epilogos' output directory
-    saliency -- The saliency metric epilogos is using
+    saliency      -- The saliency metric epilogos is using
     """
 
     jobCheckStr = "sacct --format=JobID%18,JobName%50,State%10 --jobs {}".format(allJobIDs)
 
     completedJobs = []
     calculationStep = ""
 
@@ -556,19 +538,20 @@
             print("\n Step 2: Background frequency combination\n{}\n{}\n{}"
                   .format("-" * 80, spLines[0], spLines[1]), flush=True)
             calculationStep = "exp_comb"
         elif len(completedJobs) >= (len(expJobIDArr) + 1) and calculationStep == "exp_comb":
             print("\n Step 3: Score calculation\n{}\n{}\n{}".format("-" * 80, spLines[0], spLines[1]), flush=True)
             calculationStep = "score"
         elif mode == "single" and len(completedJobs) >= (len(expJobIDArr) + 1 + len(scoreJobIDArr)) \
-                              and calculationStep == "score":
-            print("\n Step 4: Finding greatest hits\n{}\n{}\n{}".format("-" * 80, spLines[0], spLines[1]), flush=True)
-            calculationStep = "hits"
+                and calculationStep == "score":
+            print("\n Step 4: Finding regions of interest\n{}\n{}\n{}".format("-" * 80, spLines[0], spLines[1]),
+                  flush=True)
+            calculationStep = "roi"
         elif mode == "paired" and len(completedJobs) >= (len(expJobIDArr) + 1 + len(scoreJobIDArr)) \
-                              and calculationStep == "score":
+                and calculationStep == "score":
             print("\n Step 4: Generating p-values and figures\n{}\n{}\n{}"
                   .format("-" * 80, spLines[0], spLines[1]), flush=True)
             calculationStep = "visual"
 
         # Print out jobs when they are completed
         for line in spLines[2:]:
             if "COMPLETED" in line and "allocation" not in line:
@@ -587,20 +570,59 @@
             break
 
         # If final job is done, exit the program
         # Checks are if the 3rd line is not empty, if there are no more running or pending values,
         # and if an "allocation" job is not in the output
         if spLines[2] and not ("RUNNING" in sp.stdout or "PENDING" in sp.stdout) and "allocation" not in sp.stdout:
             print("\nAll jobs finished successfully. Please find output in: {}".format(outputDirPath))
-            print("\nPlease find output and error logs in {} and {} respectively\n".format(outputDirPath / ".out", "/.err"))
+            print("\nPlease find output and error logs in {} and /.err respectively\n".format(outputDirPath / ".out"))
             break
 
         # Don't want to spam cluster with commands so sleep
         # Sleep less time for saliency one since it is much faster
         if saliency == 1:
             sleep(2)
         else:
             sleep(10)
 
 
+def determineMemories(numProcesses, expFreqMem, expCombMem, scoreMem, roiMem, mode):
+    """
+    Generates memory strings for slurm commands
+
+    Input:
+    numProcesses -- The number of cores the user would like to use
+    expFreqMem   -- The memory (in MB) to be used for the expected frequency calculations
+    expCombMem   -- The memory (in MB) to be used for the expected frequency calculations
+    scoreMem     -- The memory (in MB) to be used for the expected frequency calculations
+    roiMem       -- The memory (in MB) to be used for the expected frequency calculations
+    mode         -- 'single' or 'paired'; tells us which version of epilogos we are running
+
+    Output:
+    expFreqMem -- A string for slurm commands containing information on ntasks and memory (for exp freq calculation)
+    expCombMem -- A string for slurm commands containing information on ntasks and memory (for exp comb calculation)
+    scoreMem   -- A string for slurm commands containing information on ntasks and memory (for score calculation)
+    roiMem     -- A string for slurm commands containing information on ntasks and memory (for roi calculation)
+    """
+
+    # 0 cores is defined to take all resources on node
+    if numProcesses == 0:
+        expFreqMem, expCombMem, scoreMem, roiMem = "--exclusive --mem=0"
+    else:
+        expFreqMem = "--ntasks={} --mem={}".format(numProcesses, expFreqMem)
+        expCombMem = "--ntasks={} --mem={}".format(numProcesses, expCombMem)
+        scoreMem   = "--ntasks={} --mem={}".format(numProcesses, scoreMem)
+
+        # Default roi memory is different for single/paired mode
+        if roiMem == -1:
+            if mode == "single":
+                roiMem = "--ntasks={} --mem=20000".format(numProcesses)
+            else:
+                roiMem = "--ntasks={} --mem=100000".format(numProcesses)
+        else:
+            roiMem = "--ntasks={} --mem={}".format(numProcesses, roiMem)
+
+    return expFreqMem, expCombMem, scoreMem, roiMem
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `epilogos-0.1.1/epilogos/scores.py` & `epilogos-0.1.2/epilogos/scores.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,34 +3,35 @@
 from pathlib import Path
 import pandas as pd
 from time import time
 import numpy.ma as ma
 from multiprocessing import cpu_count, Pool, RawArray
 from itertools import repeat, permutations
 from contextlib import closing
-from epilogos.helpers import strToBool, splitRows, readStates
+from epilogos.helpers import strToBool, countRows, splitRows, readStates, sharedToNumpy
 import gzip
 
 
-def main(file1, file2, numStates, saliency, outputDir, expFreqPath, fileTag, numProcesses, quiescentState, groupSize, verbose):
+def main(file1, file2, numStates, saliency, outputDir, expFreqPath, fileTag, numProcesses, quiescentState, groupSize,
+         verbose):
     """
     Wrapper function which prepares inputs for the score calculation
 
     Input:
-    file1 -- The path of the only (single epilogos) or first (paired epilogos) file to read states from
-    file2 -- The path of the second file to read states from (paired epilogos)
-    numStates -- The number of states in the state model
-    saliency -- The saliency metric being used in the epilogos run
-    outputDir -- The path of the output directory
-    expFreqPath -- The path of the expected frequency array
-    fileTag -- A string which helps ensure outputed files are named similarly within an epilogos run
-    numProcesses -- The number of cores to run on
+    file1          -- The path of the only (single epilogos) or first (paired epilogos) file to read states from
+    file2          -- The path of the second file to read states from (paired epilogos)
+    numStates      -- The number of states in the state model
+    saliency       -- The saliency metric being used in the epilogos run
+    outputDir      -- The path of the output directory
+    expFreqPath    -- The path of the expected frequency array
+    fileTag        -- A string which helps ensure outputed files are named similarly within an epilogos run
+    numProcesses   -- The number of cores to run on
     quiescentState -- The state used to filter out quiescent bins
-    groupSize -- Size of the outputted null array
-    verbose -- Boolean which if True, causes much more detailed prints
+    groupSize      -- Size of the outputted null array
+    verbose        -- Boolean which if True, causes much more detailed prints
     """
     if verbose: tTotal = time()
 
     file1Path = Path(file1)
     file2Path = Path(file2)
     outputDirPath = Path(outputDir)
 
@@ -39,46 +40,34 @@
     if not verbose: print("    {}\t".format(filename), end="", flush=True)
 
     # If user doesn't want to choose number of cores use as many as available
     if numProcesses == 0:
         numProcesses = cpu_count()
 
     # Determine which rows to assign to each core
-    rowList = splitRows(file1Path, numProcesses)
+    rowList = splitRows(countRows(file1Path), numProcesses)
 
     if file2 == "null":
-        calculateScores(saliency, file1Path, rowList, numStates, outputDirPath, expFreqPath, fileTag, filename, numProcesses,
-                        verbose)
+        calculateScores(saliency, file1Path, rowList, numStates, outputDirPath, expFreqPath, fileTag, filename,
+                        numProcesses, verbose)
     else:
         calculateScoresPairwise(saliency, file1Path, file2Path, rowList, numStates, outputDirPath, expFreqPath, fileTag,
                                 filename, numProcesses, quiescentState, groupSize, verbose)
 
     print("Total Time:", time() - tTotal, flush=True) if verbose else print("\t[Done]", flush=True)
 
 
-def sharedToNumpy(sharedArr, numRows, numStates):
-    """
-    Helper for unflattening a shared array into a 2d numpy array
-
-    Input:
-    sharedArr -- The shared array to shape
-    numRows -- The number of rows for the numpy array
-    numStates -- The number of columns for the numpy array
-    """
-    return np.frombuffer(sharedArr, dtype=np.float32).reshape((numRows, numStates))
-
-
 def _init(sharedArr_, expFreqPath_, verbose_):
     """
     Initializes global variables for multiprocessing in the single epilogos case
 
     Input:
-    sharedArr_ -- A tuple containing relevant information about the shared score array
+    sharedArr_   -- A tuple containing relevant information about the shared score array
     expFreqPath_ -- A pathlib path to the expected frequency array
-    verbose_ -- A boolean which tells us the amount we need to print
+    verbose_     -- A boolean which tells us the amount we need to print
     """
     global sharedArr
     global expFreqPath
     global verbose
 
     sharedArr = sharedArr_
     expFreqPath = expFreqPath_
@@ -87,25 +76,25 @@
 
 def _initPairwise(sharedArr1_, sharedArr2_, shuffledSharedArr1_, shuffledSharedArr2_, quiescenceSharedArr_, totalRows,
                   numStates, quiescentState_, expFreqPath_, groupSize_, verbose_):
     """
     Initializes global variables for multiprocessing in the paired epilogos case
 
     Input:
-    sharedArr1_ -- The first shared score array
-    sharedArr2_ -- The second shared score array
-    shuffledSharedArr1_ -- The first shared null score array
-    shuffledSharedArr2_ -- The second shared null score array
+    sharedArr1_          -- The first shared score array
+    sharedArr2_          -- The second shared score array
+    shuffledSharedArr1_  -- The first shared null score array
+    shuffledSharedArr2_  -- The second shared null score array
     quiescenceSharedArr_ -- Shared array containing T/F values for whether a bin is quiescent
-    totalRows -- The number of rows of the input files
-    numStates -- The number of states in the state model
-    quiescentState_ -- The state used to filter out quiescent bins
-    expFreqPath_ -- A pathlib path to the expected frequency array
-    groupSize_ -- Size of outputed null array
-    verbose_ -- A boolean which tells us the amount we need to print
+    totalRows            -- The number of rows of the input files
+    numStates            -- The number of states in the state model
+    quiescentState_      -- The state used to filter out quiescent bins
+    expFreqPath_         -- A pathlib path to the expected frequency array
+    groupSize_           -- Size of outputed null array
+    verbose_             -- A boolean which tells us the amount we need to print
     """
     global sharedArr1
     global sharedArr2
     global shuffledSharedArr1
     global shuffledSharedArr2
     global quiescenceSharedArr
     global quiescentState
@@ -120,30 +109,34 @@
     quiescenceSharedArr = quiescenceSharedArr_
     quiescentState = quiescentState_
     expFreqPath = expFreqPath_
     verbose = verbose_
     groupSize = groupSize_
 
 
-def calculateScores(saliency, file1Path, rowList, numStates, outputDirPath, expFreqPath, fileTag, filename, numProcesses,
-                    verbose):
+def calculateScores(saliency, file1Path, rowList, numStates, outputDirPath, expFreqPath, fileTag, filename,
+                    numProcesses, verbose):
     """
     Function responsible for deploying the processes used to calculate the scores in the single epilogos case
 
     Input:
-    saliency -- The saliency metric being used in the epilogos run
-    file1Path -- The path of the only file to read states from
-    rowList -- A list of tuples which contain the first and last rows for each core to use
-    numStates -- The number of states in the state model
+    saliency      -- The saliency metric being used in the epilogos run
+    file1Path     -- The path of the only file to read states from
+    rowList       -- A list of tuples which contain the first and last rows for each core to use
+    numStates     -- The number of states in the state model
     outputDirPath -- The path of the output directory
-    expFreqPath -- The path to the expected frequency array
-    fileTag -- A string which helps ensure outputed files are named similarly within an epilogos run
-    filename -- The name of the file for which we are calculating the expected frequencies
-    numProcesses -- The number of cores to run on
-    verbose -- Boolean which if True, causes much more detailed prints
+    expFreqPath   -- The path to the expected frequency array
+    fileTag       -- A string which helps ensure outputed files are named similarly within an epilogos run
+    filename      -- The name of the file for which we are calculating the expected frequencies
+    numProcesses  -- The number of cores to run on
+    verbose       -- Boolean which if True, causes much more detailed prints
+
+    Output:
+    scores*.txt.gz file containing the scores for the input file
+    temp_scores*.npz file containing the scores as a npz file for fast reading later
     """
 
     if verbose: print("\nNumber of Processes:", numProcesses, flush=True)
 
     totalRows = rowList[-1][-1]
 
     # Shared arrays across the multiple processes for the scores
@@ -159,118 +152,132 @@
             pool.starmap(s2Score, zip(repeat(file1Path), repeat(Path("null")), rowList))
         elif saliency == 3:
             pool.starmap(s3Score, zip(repeat(file1Path), rowList))
         else:
             raise ValueError("Please ensure that saliency metric is either 1, 2, or 3")
     pool.join()
 
-    chrName = pd.read_table(file1Path, nrows=1, header=None, sep="\t").iloc[0, 0]
-    locationArr = np.array([[chrName, 200*i, 200*i+200] for i in range(totalRows)])
+    # chrName = pd.read_table(file1Path, nrows=1, header=None, sep="\t").iloc[0, 0]
+    # locationArr = np.array([[chrName, 200*i, 200*i+200] for i in range(totalRows)])
+    locationArr = pd.read_table(file1Path, header=None, sep="\t", usecols=[0, 1, 2]).to_numpy()
 
     outputTxtPath = outputDirPath / "scores_{}_{}.txt.gz".format(fileTag, filename)
     writeScores(sharedToNumpy(sharedArr, totalRows, numStates), outputTxtPath, locationArr)
-    # Temporary scores for greatest hits (np files are faster to read in)
+    # Temporary scores for regions of interest (np files are faster to read in)
+    chrName = pd.read_table(file1Path, nrows=1, header=None, usecols=[0], sep="\t").iloc[0, 0]
     tempScoresPath = outputDirPath / "temp_scores_{}_{}.npz".format(fileTag, filename)
-    np.savez_compressed(tempScoresPath, chrName=np.array([chrName]), scoreArr=sharedToNumpy(sharedArr, totalRows, numStates),
-                        locationArr=locationArr)
+    np.savez_compressed(tempScoresPath, chrName=np.array([chrName]),
+                        scoreArr=sharedToNumpy(sharedArr, totalRows, numStates), locationArr=locationArr)
 
 
 def calculateScoresPairwise(saliency, file1Path, file2Path, rowList, numStates, outputDirPath, expFreqPath, fileTag,
                             filename, numProcesses, quiescentState, groupSize, verbose):
     """
     Function responsible for deploying the processes used to calculate the scores in the paired epilogos case
 
     Input:
-    saliency -- The saliency metric being used in the epilogos run
-    file1Path -- The path of the first file to read states from
-    file2Path -- The path of the second file to read states from
-    rowList -- A list of tuples which contain the first and last rows for each core to use
-    numStates -- The number of states in the state model
-    outputDirPath -- The path of the output directory
-    expFreqPath -- The path to the expected frequency array
-    fileTag -- A string which helps ensure outputed files are named similarly within an epilogos run
-    filename -- The name of the file for which we are calculating the expected frequencies
-    numProcesses -- The number of cores to run on
+    saliency       -- The saliency metric being used in the epilogos run
+    file1Path      -- The path of the first file to read states from
+    file2Path      -- The path of the second file to read states from
+    rowList        -- A list of tuples which contain the first and last rows for each core to use
+    numStates      -- The number of states in the state model
+    outputDirPath  -- The path of the output directory
+    expFreqPath    -- The path to the expected frequency array
+    fileTag        -- A string which helps ensure outputed files are named similarly within an epilogos run
+    filename       -- The name of the file for which we are calculating the expected frequencies
+    numProcesses   -- The number of cores to run on
     quiescentState -- The state used to filter out quiescent bins
-    groupSize -- Size of the outputted null array
-    verbose -- Boolean which if True, causes much more detailed prints
+    groupSize      -- Size of the outputted null array
+    verbose        -- Boolean which if True, causes much more detailed prints
+
+    Output:
+    pairwiseDelta*.txt.gz file containing the differences between the scores of input files
+    temp_nullDistances*.npz file containing the null distances as a npz file for fast reading later
+    temp_quiescence*.npz file containing booleans identifying bins which are completely quiescent
     """
     if verbose: print("\nNumber of Processes:", numProcesses, flush=True)
 
     totalRows = rowList[-1][-1]
 
     # Shared arrays across the multiple processes for the scores
     # We avoid race conditions by writing to separate parts of the array in each process
     sharedArr1 = RawArray(np.ctypeslib.as_ctypes_type(np.float32), totalRows * numStates)
     sharedArr2 = RawArray(np.ctypeslib.as_ctypes_type(np.float32), totalRows * numStates)
     shuffledSharedArr1 = RawArray(np.ctypeslib.as_ctypes_type(np.float32), totalRows * numStates)
     shuffledSharedArr2 = RawArray(np.ctypeslib.as_ctypes_type(np.float32), totalRows * numStates)
     quiescenceSharedArr = RawArray(np.ctypeslib.as_ctypes_type(np.bool_), totalRows)
 
     # Start the processes
-    with closing(Pool(numProcesses, initializer=_initPairwise, initargs=(sharedArr1, sharedArr2, shuffledSharedArr1,
-                                                                         shuffledSharedArr2, quiescenceSharedArr, totalRows,
-                                                                         numStates, quiescentState, expFreqPath, groupSize,
-                                                                         verbose))) as pool:
+    with closing(Pool(numProcesses, initializer=_initPairwise,
+                      initargs=(sharedArr1, sharedArr2, shuffledSharedArr1, shuffledSharedArr2, quiescenceSharedArr,
+                                totalRows, numStates, quiescentState, expFreqPath, groupSize, verbose))) as pool:
         if saliency == 1:
             pool.starmap(s1Score, zip(repeat(file1Path), repeat(file2Path), rowList))
         elif saliency == 2:
             pool.starmap(s2Score, zip(repeat(file1Path), repeat(file2Path), rowList))
         else:
             raise ValueError("Please ensure that saliency metric is either 1 or 2 for Pairwise Epilogos")
     pool.join()
 
     # Calculate the differences between array 1 and 2 in both the real and null case
     if verbose: print("Calculating Raw Differences...", flush=True); tDiff = time()
     realDiffArr = sharedToNumpy(sharedArr1, totalRows, numStates) - sharedToNumpy(sharedArr2, totalRows, numStates)
-    nullDiffArr = sharedToNumpy(shuffledSharedArr1, totalRows, numStates) - \
-                  sharedToNumpy(shuffledSharedArr2, totalRows, numStates)
+    nullDiffArr = sharedToNumpy(shuffledSharedArr1, totalRows, numStates)\
+        - sharedToNumpy(shuffledSharedArr2, totalRows, numStates)
     if verbose: print("    Time:", time() - tDiff, flush=True)
 
     # Only calculate the distances for the null data in this step
     if verbose: print("Calculating Squared Euclidean Distance and Maximum Contributing Difference...", flush=True); \
         tDistance = time()
     diffSign = np.sign(np.sum(nullDiffArr, axis=1))
     nullDistancesArr = np.sum(np.square(nullDiffArr), axis=1) * diffSign
     if verbose: print("    Time:", time() - tDistance, flush=True)
 
     # If it's the real data, we will just write the delta and calculate metrics in computeEpilogosPairwiseVisual
-    # If it's the null data, we will just save the signed squared euclidean distances as a temporary npz file as we don't
-    # care about saving the data
-    # We also want to write the locations of any quiescent bins (where all states are in the quiescent state). This ensures
-    # that our eventual fit on the null data is more accurate.
+    # If it's the null data, we will just save the signed squared euclidean distances as a temporary npz file as we
+    # don't care about saving the data
+    # We also want to write the locations of any quiescent bins (where all states are in the quiescent state).
+    # This ensures that our eventual fit on the null data is more accurate.
     if verbose: print("Writing output to disk...", flush=True); tWrite = time()
-    chrName = pd.read_table(file1Path, nrows=1, header=None, sep="\t").iloc[0, 0]
-    locationArr = np.array([[chrName, 200*i, 200*i+200] for i in range(totalRows)])
+
+    # chrName = pd.read_table(file1Path, nrows=1, header=None, sep="\t").iloc[0, 0]
+    # locationArr = np.array([[chrName, 200*i, 200*i+200] for i in range(totalRows)])
+    locationArr = pd.read_table(file1Path, header=None, sep="\t", usecols=[0, 1, 2]).to_numpy()
+
     realOutputPath = outputDirPath / "pairwiseDelta_{}_{}.txt.gz".format(fileTag, filename)
     writeScores(realDiffArr, realOutputPath, locationArr)
+
+    chrName = pd.read_table(file1Path, nrows=1, header=None, usecols=[0], sep="\t").iloc[0, 0]
+
     nullOutputPath = outputDirPath / "temp_nullDistances_{}_{}.npz".format(fileTag, filename)
     np.savez_compressed(nullOutputPath, chrName=np.array([chrName]), nullDistances=nullDistancesArr)
     quiescentOutputPath = outputDirPath / "temp_quiescence_{}_{}.npz".format(fileTag, filename)
     np.savez_compressed(quiescentOutputPath, chrName=np.array([chrName]),
                         quiescenceArr=np.frombuffer(quiescenceSharedArr, dtype=np.bool_))
     if verbose: print("    Time:", time() - tWrite, flush=True)
 
 
 def s1Score(file1Path, file2Path, rowsToCalc):
     """
     Function responsible for score calculation over a set of rows for a saliency metric of 1. Note that there are global
-    variables used for the shared score array(s). There is no output as scores are put directly into the shared score array(s)
+    variables used for the shared score array(s). There is no output as scores are put directly into the shared score
+    array(s)
 
     Input:
-    file1Path -- The path of the only (single epilogos) or first (paired epilogos) file to read states from
-    file2Path -- The path of the second file to read states from (paired epilogos)
+    file1Path  -- The path of the only (single epilogos) or first (paired epilogos) file to read states from
+    file2Path  -- The path of the second file to read states from (paired epilogos)
     rowsToCalc -- The rows to count expected frequencies from the files
     """
     # Loading the expected frequency array
     expFreqArr = np.load(expFreqPath, allow_pickle=False)
 
     # Loading the data and creating the shared arrays for the scores
     if str(file2Path) == "null":
-        dataArr = readStates(file1Path=file1Path, file2Path=file2Path, rowsToCalc=rowsToCalc, expBool=False, verbose=verbose)
+        dataArr = readStates(file1Path=file1Path, file2Path=file2Path, rowsToCalc=rowsToCalc, expBool=False,
+                             verbose=verbose)
 
         numStates = sharedArr[2]
 
         scoreArr = sharedToNumpy(*sharedArr)
     else:
         file1Arr, file2Arr, shuffledFile1Arr, shuffledFile2Arr = readStates(file1Path=file1Path, file2Path=file2Path,
                                                                             rowsToCalc=rowsToCalc, expBool=False,
@@ -284,15 +291,16 @@
         nullScoreArr2 = sharedToNumpy(*shuffledSharedArr2)
         quiescenceArr = np.frombuffer(quiescenceSharedArr, dtype=np.bool_)
 
         if quiescentState != -1:
             # Figure out the quiescent bins
             sortedArr1 = np.sort(file1Arr, axis=1)
             sortedArr2 = np.sort(file2Arr, axis=1)
-            # If all values in a bin are equal to the quiescentState in both file1Arr and file2Arr, then the bin is quiescent
+            # If all values in a bin are equal to the quiescentState in both file1Arr and file2Arr,
+            # then the bin is quiescent
             quiescenceArr[rowsToCalc[0]:rowsToCalc[1]][np.where((sortedArr1[:, 0] == quiescentState)
                                                                 & (sortedArr1[:, -1] == quiescentState)
                                                                 & (sortedArr2[:, 0] == quiescentState)
                                                                 & (sortedArr2[:, -1] == quiescentState))] = True
 
     if verbose and rowsToCalc[0] == 0: print("Calculating Scores...", flush=True); tScore = time(); percentDone = 0
     printCheckmarks = [int(rowsToCalc[1] * float(i / 10)) for i in range(1, 10)]
@@ -317,42 +325,47 @@
 
 
 def rowObsS1(dataArr, row, numStates):
     """
     Calculates the observed counts for each state for a saliency metric of 1
 
     Input:
-    dataArr -- The numpy array which contains the states to count
-    row -- The row from which to calculate the observed counts
+    dataArr   -- The numpy array which contains the states to count
+    row       -- The row from which to calculate the observed counts
     numStates -- The number of states in the state model
+
+    Output:
+    rowObsArr -- Observed counts for each state in a row for a saliency metric of 1
     """
     rowObsArr = np.zeros(numStates)
     # Count number of each state in row and return array
     uniqueStates, stateCounts = np.unique(dataArr[row], return_counts=True)
     for i, state in enumerate(uniqueStates):
         rowObsArr[state] = stateCounts[i] / dataArr.shape[1]
     return rowObsArr
 
 
 def s2Score(file1Path, file2Path, rowsToCalc):
     """
     Function responsible for score calculation over a set of rows for a saliency metric of 2. Note that there are global
-    variables used for the shared score array(s). There is no output as scores are put directly into the shared score array(s)
+    variables used for the shared score array(s). There is no output as scores are put directly into the shared score
+    array(s)
 
     Input:
-    file1Path -- The path of the only (single epilogos) or first (paired epilogos) file to read states from
-    file2Path -- The path of the second file to read states from (paired epilogos)
+    file1Path  -- The path of the only (single epilogos) or first (paired epilogos) file to read states from
+    file2Path  -- The path of the second file to read states from (paired epilogos)
     rowsToCalc -- The rows to count expected frequencies from the files
     """
     # Loading the expected frequency array
     expFreqArr = np.load(expFreqPath, allow_pickle=False)
 
     # Loading the data and creating the shared arrays for the scores
     if str(file2Path) == "null":
-        dataArr = readStates(file1Path=file1Path, file2Path=file2Path, rowsToCalc=rowsToCalc, expBool=False, verbose=verbose)
+        dataArr = readStates(file1Path=file1Path, file2Path=file2Path, rowsToCalc=rowsToCalc, expBool=False,
+                             verbose=verbose)
 
         numStates = sharedArr[2]
 
         scoreArr = sharedToNumpy(*sharedArr)
 
         # Need the permuations to effective count state pairs (see rowObsS2() for theory)
         permutations = dataArr.shape[1] * (dataArr.shape[1] - 1)
@@ -369,15 +382,16 @@
         nullScoreArr2 = sharedToNumpy(*shuffledSharedArr2)
         quiescenceArr = np.frombuffer(quiescenceSharedArr, dtype=np.bool_)
 
         if quiescentState != -1:
             # Figure out the quiescent bins
             sortedArr1 = np.sort(file1Arr, axis=1)
             sortedArr2 = np.sort(file2Arr, axis=1)
-            # If all values in a bin are equal to the quiescentState in both file1Arr and file2Arr, then the bin is quiescent
+            # If all values in a bin are equal to the quiescentState in both file1Arr and file2Arr, then the bin is
+            # quiescent
             quiescenceArr[rowsToCalc[0]:rowsToCalc[1]][np.where((sortedArr1[:, 0] == quiescentState)
                                                                 & (sortedArr1[:, -1] == quiescentState)
                                                                 & (sortedArr2[:, 0] == quiescentState)
                                                                 & (sortedArr2[:, -1] == quiescentState))] = True
 
         # Need the permuations to effective count state pairs (see rowObsS2() for theory)
         permutations1 = file1Arr.shape[1] * (file1Arr.shape[1] - 1)
@@ -393,57 +407,63 @@
             print("    {}% Completed".format(percentDone), flush=True)
         if not verbose and rowsToCalc[0] == 0 and obsRow in printCheckmarks: print(".", end="", flush=True)
 
         # Inputs to klScoreND are obsFreqArr and expFreqArr respectively
         if str(file2Path) == "null":
             scoreArr[scoreRow] = klScoreND(rowObsS2(dataArr, obsRow, permutations, numStates), expFreqArr).sum(axis=0)
         else:
-            realScoreArr1[scoreRow] = klScoreND(rowObsS2(file1Arr, obsRow, permutations1, numStates), expFreqArr).sum(axis=0)
-            realScoreArr2[scoreRow] = klScoreND(rowObsS2(file2Arr, obsRow, permutations2, numStates), expFreqArr).sum(axis=0)
+            realScoreArr1[scoreRow] = klScoreND(rowObsS2(file1Arr, obsRow, permutations1, numStates),
+                                                expFreqArr).sum(axis=0)
+            realScoreArr2[scoreRow] = klScoreND(rowObsS2(file2Arr, obsRow, permutations2, numStates),
+                                                expFreqArr).sum(axis=0)
             nullScoreArr1[scoreRow] = klScoreND(rowObsS2(shuffledFile1Arr, obsRow, permutations1, numStates),
                                                 expFreqArr).sum(axis=0)
             nullScoreArr2[scoreRow] = klScoreND(rowObsS2(shuffledFile2Arr, obsRow, permutations2, numStates),
                                                 expFreqArr).sum(axis=0)
 
     if verbose and rowsToCalc[0] == 0: print("    Time:", time() - tScore, flush=True)
 
 
 def rowObsS2(dataArr, row, permutations, numStates):
     """
     Calculates the observed counts for each pair of states for a saliency metric of 2
 
     Input:
-    dataArr -- The numpy array which contains the states to count
-    row -- The row from which to calculate the observed counts
+    dataArr      -- The numpy array which contains the states to count
+    row          -- The row from which to calculate the observed counts
     permutations -- The number of permutations of epigenomes possible within the row of the dataArr
-    numStates -- The number of states in the state model
+    numStates    -- The number of states in the state model
+
+    Output:
+    rowObsArr -- Observed counts for each pair of states within a bin for a saliency metric of 2
     """
-    # (Within a row, how many ways can you choose x and y to be together) / (how many ordered ways can you choose 2 states)
+    # (Within a row, # of ways can you choose x and y to be together) / (# of ordered ways can you choose 2 states)
     #  = Prob of choosing x and y
     # Can choose x and y to be together x*y ways if different and n(n-1) ways if same
     # (where n is the number of times that x/y shows up)
     rowObsArr = np.zeros((numStates, numStates))
     uniqueStates, stateCounts = np.unique(dataArr[row], return_counts=True)
     for i, state1 in enumerate(uniqueStates):
         for j, state2 in enumerate(uniqueStates):
             if state1 == state2:
                 # Equates to statecounts[i] permute 2 / permutations
-                rowObsArr[state1, state2] = stateCounts[i] * (stateCounts[i] - 1) / permutations
+                rowObsArr[state1, state2] = stateCounts[i] * (stateCounts[j] - 1) / permutations
             else:  # state1 > state2 or state1 < state2
                 rowObsArr[state1, state2] = stateCounts[i] * stateCounts[j] / permutations
     return rowObsArr
 
 
 def s3Score(file1Path, rowsToCalc):
     """
     Function responsible for score calculation over a set of rows for a saliency metric of 3. Note that there are global
-    variables used for the shared score array(s). There is no output as scores are put directly into the shared score array(s)
+    variables used for the shared score array(s). There is no output as scores are put directly into the shared score
+    array(s)
 
     Input:
-    file1Path -- The path of the only file to read states from
+    file1Path  -- The path of the only file to read states from
     rowsToCalc -- The rows to count expected frequencies from the files
     """
     dataArr = readStates(file1Path=file1Path, rowsToCalc=rowsToCalc, verbose=verbose)
 
     # Loading the expected frequency array
     expFreqArr = np.load(expFreqPath, allow_pickle=False)
 
@@ -452,16 +472,16 @@
 
     # Gives us everyway to combine the column numbers in numpy indexing form
     basePermutationArr = np.array(list(permutations(range(numCols), 2)), dtype=np.int16).T
 
     # Because each epigenome, epigenome, state, state combination only occurs once per row, we can precalculate all the
     # scores assuming a frequency of 1/(numCols*(numCols-1))
     # This saves a lot of time in the loop as we are just looking up references and not calculating
-    scoreArrOnes = klScoreND(np.ones((numCols, numCols, numStates, numStates), dtype=np.float32) / (numCols * (numCols - 1)),
-                             expFreqArr)
+    scoreArrOnes = klScoreND(np.ones((numCols, numCols, numStates, numStates), dtype=np.float32)
+                             / (numCols * (numCols - 1)), expFreqArr)
 
     if verbose and rowsToCalc[0] == 0: print("Calculating Scores...", flush=True); tScore = time(); percentDone = 0
     printCheckmarks = [int(rowsToCalc[1] * float(i / 10)) for i in range(1, 10)]
 
     # Calculte the scores and store them in the shared array
     scoreArr = sharedToNumpy(*sharedArr)
     rowScoreArr = np.zeros(numStates, dtype=np.float32)
@@ -469,18 +489,17 @@
 
         if verbose and rowsToCalc[0] == 0 and dataRow in printCheckmarks: percentDone += 10; \
             print("    {}% Completed".format(percentDone), flush=True)
         if not verbose and rowsToCalc[0] == 0 and dataRow in printCheckmarks: print(".", end="", flush=True)
 
         if dataRow < dataArr.shape[0]:
             # Pull the scores from the precalculated score array add them to the correct index in the rowScoreArr
-            np.add.at(rowScoreArr, dataArr[dataRow, basePermutationArr[1]], scoreArrOnes[basePermutationArr[0],
-                                                                                    basePermutationArr[1],
-                                                                                    dataArr[dataRow, basePermutationArr[0]],
-                                                                                    dataArr[dataRow, basePermutationArr[1]]])
+            np.add.at(rowScoreArr, dataArr[dataRow, basePermutationArr[1]],
+                      scoreArrOnes[basePermutationArr[0], basePermutationArr[1],
+                                   dataArr[dataRow, basePermutationArr[0]], dataArr[dataRow, basePermutationArr[1]]])
 
             # Store the scores in the shared score array
             scoreArr[scoreRow] = rowScoreArr
 
             # Reset the array so it doesn't carry over scores from other rows
             rowScoreArr.fill(0)
 
@@ -491,24 +510,29 @@
     """
     Writes the scores out to a gziped text file
 
     Input:
     dataArr -- Numpy array containing the scores to write
     outputTextPath -- The path of the file to write to
     locationArr -- Numpy array containing the genomic locations of the scores
+
+    Output:
+    scores*.txt.gz file containing the scores for the input file
+    OR
+    pairwiseDelta*.txt.gz file containing the differences between the scores of input files
     """
     outputTxt = gzip.open(outputTxtPath, "wt")
 
     # Create a location array
     numRows = dataArr.shape[0]
     numStates = dataArr.shape[1]
 
     # Creating a string to write out the data (faster than np.savetxt)
-    outputTemplate = "{0[0]}\t{0[1]}\t{0[2]}\t" + "".join("{1[%d]:.5f}\t" % i for i in range(numStates - 1)) + \
-                     "{1[%d]:.5f}\n" % (numStates - 1)
+    outputTemplate = "{0[0]}\t{0[1]}\t{0[2]}\t" + "".join("{1[%d]:.5f}\t" % i for i in range(numStates - 1))\
+                     + "{1[%d]:.5f}\n" % (numStates - 1)
     outputStr = "".join(outputTemplate.format(locationArr[i], dataArr[i]) for i in range(numRows))
 
     # Write out the string
     outputTxt.write(outputStr)
     outputTxt.close()
 
 
@@ -523,9 +547,9 @@
     Output:
     Nd numpy array with the kullback leibler scores
     """
     return obs * ma.log2(ma.divide(obs, exp).filled(0)).filled(0)
 
 
 if __name__ == "__main__":
-    main(argv[1], argv[2], int(argv[3]), int(argv[4]), argv[5], argv[6], argv[7], int(argv[8]), int(argv[9]), int(argv[10]),
-         strToBool(argv[11]))
+    main(argv[1], argv[2], int(argv[3]), int(argv[4]), argv[5], argv[6], argv[7], int(argv[8]), int(argv[9]),
+         int(argv[10]), strToBool(argv[11]))
```

### Comparing `epilogos-0.1.1/epilogos.egg-info/PKG-INFO` & `epilogos-0.1.2/epilogos.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,87 @@
 Metadata-Version: 2.1
 Name: epilogos
-Version: 0.1.1
+Version: 0.1.2
 Summary: Information-theoretic navigation of multi-tissue functional genomic annotations
 Home-page: https://github.com/meuleman/epilogos
 Author: Wouter Meuleman, Jacob Quon, Alex Reynolds, Eric Rynes
 Author-email: wouter@meuleman.org
 License: LICENSE.txt
-Description: .. image:: https://raw.githubusercontent.com/meuleman/epilogos/main/data/logo.png
-          :width: 840
-          :alt: Epilogos
-        
-        ------
-        
-        
-        Information-theoretic navigation of multi-tissue functional genomic annotations
-        ===============================================================================
-        
-        Epilogos is an approach for analyzing, visualizing, and navigating multi-biosample functional genomic annotations, with an emphasis on chromatin state maps generated with e.g. ChromHMM or Segway.
-        
-        The software provided in this repository implements the methods underlying Epilogos using Python 3.7. We provide a proof-of-principle dataset based on chromatin state calls from the EpiMap dataset (`Boix et al., Nature 2021 <https://www.nature.com/articles/s41586-020-03145-z>`_).
-        
-        Created by: Wouter Meuleman, Jacob Quon, Alex Reynolds, and Eric Rynes
-        
-        ------
-        
-        
-        Installation
-        ============
-        
-        Although not required, it is good practice to create a virtual environment in which
-        specific versions of Python and its libraries are installed.
-        This can be done using ``conda``, for instance as such:
-        
-        .. code-block:: bash
-        
-            $ conda init bash  ## only needed upon first use of conda. Restart shell after this.
-            $ conda create -n epilogos python=3.8
-            $ conda activate epilogos
-        
-        To install Epilogos simply run the following command
-        
-        .. code-block:: bash
-        
-            $ pip install epilogos
-        
-        Alternatively, install Epilogos directly from the Git repositority using
-        
-        .. code-block:: bash
-        
-            $ pip install git+https://github.com/meuleman/epilogos
-        
-        
-        Prerequisites
-        =============
-        
-        To compute epilogos, you will need to have the following python libraries installed: `cython <https://cython.org/>`_, `pyranges <https://github.com/biocore-ntnu/pyranges>`_, `statsmodels <https://www.statsmodels.org/stable/index.html>`_, `click <https://click.palletsprojects.com/en/7.x/>`_, `numpy <https://numpy.org/>`_, `scipy <https://www.scipy.org/>`_, `matplotlib <https://matplotlib.org/stable/index.html>`_, and `pandas <https://pandas.pydata.org/>`_. These can be installed with one of the following commands
-        
-        .. code-block:: bash
-        
-            $ pip install 'cython>=0.29.23,<1.0.0'; pip install 'click>=7.1.2,<8.0.0' 'numpy>=1.19.2,<2.0.0' 'pandas>=1.1.3,<2.0.0' 'pyranges>=0.0.97,<1.0.0' 'scipy>=1.5.2,<2.0.0' 'matplotlib>=3.3.2,<4.0.0' 'statsmodels>=0.12.0,<1.0.0'
-        
-        or while in the epilogos directory (we use cat and xargs to ensure installation order as pyranges is dependent on cython)
-        
-        .. code-block:: bash
-        
-            $ cat requirements.txt | xargs -n 1 -L 1 pip install
-        
-        
-        Additionally, it is recommended that python is updated to version 3.7 or later. In earlier python versions, ``src/scores.py`` may raise an OSError 16. It is worth noting that in our testing this error has not affected the results.
-        
-        
-        Running Epilogos
-        ================
-        
-        To be presented with basic documentation of arguments needed to run epilogos, simply run the command ``epilogos --help`` or ``python -m epilogos --help`` (More in-depth explanation is given on the `github README <https://github.com/meuleman/epilogos)>`_).
-        
-        By default, Epilogos assumes access to a computational cluster managed by `SLURM <https://slurm.schedmd.com/>`_.
-        A version of epilogos has been created for those without access to a SLURM cluster and can be run by using the ``-l`` flag to your command (e.g. ``epilogos -l``).
-        
-        --------------
-        
-        For a more extensive set of documentation, please refer to `our github <https://github.com/meuleman/epilogos>`_.
-        
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+.. image:: https://raw.githubusercontent.com/meuleman/epilogos/main/data/logo.png
+  :width: 840
+  :alt: Epilogos
+
+------
+
+
+Information-theoretic navigation of multi-tissue functional genomic annotations
+===============================================================================
+
+Epilogos is an approach for analyzing, visualizing, and navigating multi-biosample functional genomic annotations, with an emphasis on chromatin state maps generated with e.g. ChromHMM or Segway.
+
+The software provided in this repository implements the methods underlying Epilogos using Python 3.9. We provide a proof-of-principle dataset based on chromatin state calls from the EpiMap dataset (`Boix et al., Nature 2021 <https://www.nature.com/articles/s41586-020-03145-z>`_).
+
+Created by: Wouter Meuleman, Jacob Quon, Alex Reynolds, and Eric Rynes
+
+------
+
+
+Installation
+============
+
+Although not required, it is good practice to create a virtual environment in which
+specific versions of Python and its libraries are installed.
+This can be done using ``conda``, for instance as such:
+
+.. code-block:: bash
+
+    $ conda init bash  ## only needed upon first use of conda. Restart shell after this.
+    $ conda create -n epilogos python=3.9
+    $ conda activate epilogos
+
+To install Epilogos simply run the following two commands
+
+.. code-block:: bash
+
+    $ pip install epilogos
+
+Alternatively, install Epilogos directly from the Git repositority using
+
+.. code-block:: bash
+
+    $ pip install git+https://github.com/meuleman/epilogos
+
+
+Prerequisites
+=============
+
+To compute epilogos, you will need to have the following python libraries installed: `statsmodels <https://www.statsmodels.org/stable/index.html>`_, `click <https://click.palletsprojects.com/en/7.x/>`_, `numpy <https://numpy.org/>`_, `scipy <https://www.scipy.org/>`_, `matplotlib <https://matplotlib.org/stable/index.html>`_, `pandas <https://pandas.pydata.org/>`_, `pysam <https://pysam.readthedocs.io/en/latest/api.html>`_, `scikit-learn <https://scikit-learn.org/stable/>`_, `natsort <https://natsort.readthedocs.io/en/stable/>`_, `pyranges <https://pyranges.readthedocs.io/en/latest/autoapi/pyranges/index.html>`_, and `rich <https://rich.readthedocs.io/en/stable/index.html>`_.
+These can be installed with one of the following commands
+
+.. code-block:: bash
+
+    $ pip install 'click==8.1.3' 'numpy==1.23.4' 'pandas==1.5.1' 'scipy==1.9.3' 'matplotlib==3.6.1' 'statsmodels==0.13.2' 'scikit-learn==1.1.3' 'pysam==0.19.1' 'natsort==8.2.0' 'pyranges==0.0.117' 'rich==12.6.0'
+
+or while in the epilogos directory
+
+.. code-block:: bash
+
+    $ pip install -r requirements.txt
+
+
+Additionally, it is recommended that python is updated to version 3.9 or later. We cannot guarantee the validity of results generated by earlier verions of python.
+
+
+Running Epilogos
+================
+
+To be presented with basic documentation of arguments needed to run epilogos, simply run the command ``epilogos --help`` or ``python -m epilogos --help`` (More in-depth explanation is given on the `github README <https://github.com/meuleman/epilogos)>`_).
+
+By default, Epilogos assumes access to a computational cluster managed by `SLURM <https://slurm.schedmd.com/>`_.
+A version of epilogos has been created for those without access to a SLURM cluster and can be run by using the ``-l`` flag to your command (e.g. ``epilogos -l``).
+
+--------------
+
+For a more extensive set of documentation, please refer to `our github <https://github.com/meuleman/epilogos>`_.
```

### Comparing `epilogos-0.1.1/epilogos.egg-info/SOURCES.txt` & `epilogos-0.1.2/epilogos.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 CHANGES.txt
+LICENSE
 MANIFEST.in
 README.txt
 requirements.txt
 setup.py
 bin/download_example_data.sh
 bin/preprocess_data_ChromHMM.sh
 epilogos/__init__.py
 epilogos/expected.py
 epilogos/expectedCombination.py
-epilogos/greatestHits.py
+epilogos/filter_regions.py
 epilogos/helpers.py
-epilogos/pairwiseVisual.py
+epilogos/plotRegion.py
+epilogos/roiAndVisualPairwise.py
+epilogos/roiSingle.py
 epilogos/run.py
 epilogos/scores.py
-epilogos/test.py
+epilogos/similaritySearch_calc.py
+epilogos/similaritySearch_max_mean.py
+epilogos/similaritySearch_run.py
+epilogos/similaritySearch_write.py
 epilogos.egg-info/PKG-INFO
 epilogos.egg-info/SOURCES.txt
 epilogos.egg-info/dependency_links.txt
 epilogos.egg-info/entry_points.txt
 epilogos.egg-info/requires.txt
 epilogos.egg-info/top_level.txt
```

### Comparing `epilogos-0.1.1/setup.py` & `epilogos-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,10 +25,12 @@
     packages=find_packages("."),
     scripts=["bin/preprocess_data_ChromHMM.sh", "bin/download_example_data.sh"],
     include_package_data=True,
     install_requires=install_requirements,
     entry_points={
         "console_scripts": [
             "epilogos = epilogos.run:main",
+            "simsearch = epilogos.similaritySearch_run:main",
+            "plotregion = epilogos.plotRegion:main"
         ],
     }
-)
+)
```

