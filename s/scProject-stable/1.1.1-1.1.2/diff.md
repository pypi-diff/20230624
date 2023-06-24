# Comparing `tmp/scProject-stable-1.1.1.tar.gz` & `tmp/scProject-stable-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scProject-stable-1.1.1.tar", last modified: Sat Jun 24 19:04:04 2023, max compression
+gzip compressed data, was "scProject-stable-1.1.2.tar", last modified: Sat Jun 24 19:08:49 2023, max compression
```

## Comparing `scProject-stable-1.1.1.tar` & `scProject-stable-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 WHITEKNIGHT2022   (501) staff       (20)        0 2023-06-24 19:04:04.462257 scProject-stable-1.1.1/
--rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     1065 2023-06-24 18:59:43.000000 scProject-stable-1.1.1/LICENSE
--rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     3308 2023-06-24 19:04:04.462468 scProject-stable-1.1.1/PKG-INFO
--rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     2852 2023-06-24 19:03:01.000000 scProject-stable-1.1.1/README.md
-drwxr-xr-x   0 WHITEKNIGHT2022   (501) staff       (20)        0 2023-06-24 19:04:04.450042 scProject-stable-1.1.1/scProject/
--rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)       76 2023-06-24 18:59:43.000000 scProject-stable-1.1.1/scProject/__init__.py
--rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     5929 2023-06-24 18:59:43.000000 scProject-stable-1.1.1/scProject/matcher.py
--rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     4572 2023-06-24 18:59:43.000000 scProject-stable-1.1.1/scProject/rg.py
--rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)    19458 2023-06-24 18:59:43.000000 scProject-stable-1.1.1/scProject/stats.py
--rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)    19166 2023-06-24 18:59:49.000000 scProject-stable-1.1.1/scProject/viz.py
-drwxr-xr-x   0 WHITEKNIGHT2022   (501) staff       (20)        0 2023-06-24 19:04:04.461686 scProject-stable-1.1.1/scProject_stable.egg-info/
--rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     3308 2023-06-24 19:04:04.000000 scProject-stable-1.1.1/scProject_stable.egg-info/PKG-INFO
--rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)      330 2023-06-24 19:04:04.000000 scProject-stable-1.1.1/scProject_stable.egg-info/SOURCES.txt
--rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)        1 2023-06-24 19:04:04.000000 scProject-stable-1.1.1/scProject_stable.egg-info/dependency_links.txt
--rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     1829 2023-06-24 19:04:04.000000 scProject-stable-1.1.1/scProject_stable.egg-info/requires.txt
--rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)       10 2023-06-24 19:04:04.000000 scProject-stable-1.1.1/scProject_stable.egg-info/top_level.txt
--rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)       79 2023-06-24 19:04:04.463332 scProject-stable-1.1.1/setup.cfg
--rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)      759 2023-06-24 19:01:30.000000 scProject-stable-1.1.1/setup.py
+drwxr-xr-x   0 WHITEKNIGHT2022   (501) staff       (20)        0 2023-06-24 19:08:49.311433 scProject-stable-1.1.2/
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     1065 2023-06-24 18:59:43.000000 scProject-stable-1.1.2/LICENSE
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     3084 2023-06-24 19:08:49.311639 scProject-stable-1.1.2/PKG-INFO
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     2628 2023-06-24 19:07:47.000000 scProject-stable-1.1.2/README.md
+drwxr-xr-x   0 WHITEKNIGHT2022   (501) staff       (20)        0 2023-06-24 19:08:49.307373 scProject-stable-1.1.2/scProject/
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)       76 2023-06-24 18:59:43.000000 scProject-stable-1.1.2/scProject/__init__.py
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     5929 2023-06-24 18:59:43.000000 scProject-stable-1.1.2/scProject/matcher.py
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     4572 2023-06-24 18:59:43.000000 scProject-stable-1.1.2/scProject/rg.py
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)    19458 2023-06-24 18:59:43.000000 scProject-stable-1.1.2/scProject/stats.py
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)    19166 2023-06-24 18:59:49.000000 scProject-stable-1.1.2/scProject/viz.py
+drwxr-xr-x   0 WHITEKNIGHT2022   (501) staff       (20)        0 2023-06-24 19:08:49.310965 scProject-stable-1.1.2/scProject_stable.egg-info/
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     3084 2023-06-24 19:08:49.000000 scProject-stable-1.1.2/scProject_stable.egg-info/PKG-INFO
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)      330 2023-06-24 19:08:49.000000 scProject-stable-1.1.2/scProject_stable.egg-info/SOURCES.txt
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)        1 2023-06-24 19:08:49.000000 scProject-stable-1.1.2/scProject_stable.egg-info/dependency_links.txt
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     1829 2023-06-24 19:08:49.000000 scProject-stable-1.1.2/scProject_stable.egg-info/requires.txt
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)       10 2023-06-24 19:08:49.000000 scProject-stable-1.1.2/scProject_stable.egg-info/top_level.txt
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)       79 2023-06-24 19:08:49.312323 scProject-stable-1.1.2/setup.cfg
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)      759 2023-06-24 19:06:07.000000 scProject-stable-1.1.2/setup.py
```

### Comparing `scProject-stable-1.1.1/LICENSE` & `scProject-stable-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scProject-stable-1.1.1/PKG-INFO` & `scProject-stable-1.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scProject-stable
-Version: 1.1.1
+Version: 1.1.2
 Summary: Transfer learning framework for single cell gene expression analysis in Python
 Home-page: https://github.com/gofflab/scProject
 Author: Asher Baraban, Charles Shin, Genevieve Stein-O'Brien, Loyal Goff
 Author-email: asher.baraban@wustl.edu, cshin12@jhu.edu
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 # scProject # 
 
 <img src="https://raw.githubusercontent.com/gofflab/scProject/master/docs/scProject-logo.jpg">
 
 ## Overview ##
 
 Transfer learning for gene expression signatures (Python implementation of ProjectR).  
-Current version: 1.1.1 ([PYPI](https://pypi.org/project/scProject-stable/))
+Current version: 1.1.2 ([PYPI](https://pypi.org/project/scProject-stable/))
 
 ## Description ##
 
 scProject is a software package that allows biologists to use transfer learning to understand the usage of previously discovered features in genomic datasets. Tools like NNMF allow biologists to find a set of vectors that linearly combine to approximately reconstruct a dataset. These features can have biological meaning as a pathway, cell type, gene program, cell feature, etc.  
 
 scProject leverages scikit-learn’s and scipy’s regression tools to effectively perform a change of basis with the new basis being the features discovered from NNMF or another previous analysis tool. For example, the values in the first column of the pattern matrix are the coefficients of the features to approximate the first sample in the dataset. This analysis allows the user to see the usage of features from a previously examined dataset and see if those same features are utilized in a new dataset. Using UMAP-learn to decrease the dimensionality of the regressed pattern matrix allows the user to visualize the pattern matrix in intuitive and informative ways.  
 
@@ -53,18 +53,12 @@
 scProject API | https://scproject.readthedocs.io/en/master/contents.html
 Regression    | https://scproject.readthedocs.io/en/master/contents.html#module-scProject.rg
 Visualization | https://scproject.readthedocs.io/en/master/contents.html#module-scProject.viz
 Statistics    | https://scproject.readthedocs.io/en/master/contents.html#module-scProject.stats
 Utilities     | https://scproject.readthedocs.io/en/master/contents.html#module-scProject.matcher
 Tutorial      | https://scproject.readthedocs.io/en/master/tutorial.html
 
-## Indices and tables ##
-
-Name          | Link
-------------- | -------------
-Module Index  | https://scproject.readthedocs.io/en/master/py-modindex.html
-Search Page   | https://scproject.readthedocs.io/en/master/search.html
 
 ## Additional Information ##
 
 For more instructions and guidelines, read the [documentation](https://scproject.readthedocs.io/en/master/).  
 If you would like to leave a feedback, please contact [cshin12@jhu.edu](mailto:cshin12@jhu.edu).
```

### Comparing `scProject-stable-1.1.1/README.md` & `scProject-stable-1.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # scProject # 
 
 <img src="https://raw.githubusercontent.com/gofflab/scProject/master/docs/scProject-logo.jpg">
 
 ## Overview ##
 
 Transfer learning for gene expression signatures (Python implementation of ProjectR).  
-Current version: 1.1.1 ([PYPI](https://pypi.org/project/scProject-stable/))
+Current version: 1.1.2 ([PYPI](https://pypi.org/project/scProject-stable/))
 
 ## Description ##
 
 scProject is a software package that allows biologists to use transfer learning to understand the usage of previously discovered features in genomic datasets. Tools like NNMF allow biologists to find a set of vectors that linearly combine to approximately reconstruct a dataset. These features can have biological meaning as a pathway, cell type, gene program, cell feature, etc.  
 
 scProject leverages scikit-learn’s and scipy’s regression tools to effectively perform a change of basis with the new basis being the features discovered from NNMF or another previous analysis tool. For example, the values in the first column of the pattern matrix are the coefficients of the features to approximate the first sample in the dataset. This analysis allows the user to see the usage of features from a previously examined dataset and see if those same features are utilized in a new dataset. Using UMAP-learn to decrease the dimensionality of the regressed pattern matrix allows the user to visualize the pattern matrix in intuitive and informative ways.  
 
@@ -41,18 +41,12 @@
 scProject API | https://scproject.readthedocs.io/en/master/contents.html
 Regression    | https://scproject.readthedocs.io/en/master/contents.html#module-scProject.rg
 Visualization | https://scproject.readthedocs.io/en/master/contents.html#module-scProject.viz
 Statistics    | https://scproject.readthedocs.io/en/master/contents.html#module-scProject.stats
 Utilities     | https://scproject.readthedocs.io/en/master/contents.html#module-scProject.matcher
 Tutorial      | https://scproject.readthedocs.io/en/master/tutorial.html
 
-## Indices and tables ##
-
-Name          | Link
-------------- | -------------
-Module Index  | https://scproject.readthedocs.io/en/master/py-modindex.html
-Search Page   | https://scproject.readthedocs.io/en/master/search.html
 
 ## Additional Information ##
 
 For more instructions and guidelines, read the [documentation](https://scproject.readthedocs.io/en/master/).  
 If you would like to leave a feedback, please contact [cshin12@jhu.edu](mailto:cshin12@jhu.edu).
```

### Comparing `scProject-stable-1.1.1/scProject/matcher.py` & `scProject-stable-1.1.2/scProject/matcher.py`

 * *Files identical despite different names*

### Comparing `scProject-stable-1.1.1/scProject/rg.py` & `scProject-stable-1.1.2/scProject/rg.py`

 * *Files identical despite different names*

### Comparing `scProject-stable-1.1.1/scProject/stats.py` & `scProject-stable-1.1.2/scProject/stats.py`

 * *Files identical despite different names*

### Comparing `scProject-stable-1.1.1/scProject/viz.py` & `scProject-stable-1.1.2/scProject/viz.py`

 * *Files identical despite different names*

### Comparing `scProject-stable-1.1.1/scProject_stable.egg-info/PKG-INFO` & `scProject-stable-1.1.2/scProject_stable.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scProject-stable
-Version: 1.1.1
+Version: 1.1.2
 Summary: Transfer learning framework for single cell gene expression analysis in Python
 Home-page: https://github.com/gofflab/scProject
 Author: Asher Baraban, Charles Shin, Genevieve Stein-O'Brien, Loyal Goff
 Author-email: asher.baraban@wustl.edu, cshin12@jhu.edu
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 # scProject # 
 
 <img src="https://raw.githubusercontent.com/gofflab/scProject/master/docs/scProject-logo.jpg">
 
 ## Overview ##
 
 Transfer learning for gene expression signatures (Python implementation of ProjectR).  
-Current version: 1.1.1 ([PYPI](https://pypi.org/project/scProject-stable/))
+Current version: 1.1.2 ([PYPI](https://pypi.org/project/scProject-stable/))
 
 ## Description ##
 
 scProject is a software package that allows biologists to use transfer learning to understand the usage of previously discovered features in genomic datasets. Tools like NNMF allow biologists to find a set of vectors that linearly combine to approximately reconstruct a dataset. These features can have biological meaning as a pathway, cell type, gene program, cell feature, etc.  
 
 scProject leverages scikit-learn’s and scipy’s regression tools to effectively perform a change of basis with the new basis being the features discovered from NNMF or another previous analysis tool. For example, the values in the first column of the pattern matrix are the coefficients of the features to approximate the first sample in the dataset. This analysis allows the user to see the usage of features from a previously examined dataset and see if those same features are utilized in a new dataset. Using UMAP-learn to decrease the dimensionality of the regressed pattern matrix allows the user to visualize the pattern matrix in intuitive and informative ways.  
 
@@ -53,18 +53,12 @@
 scProject API | https://scproject.readthedocs.io/en/master/contents.html
 Regression    | https://scproject.readthedocs.io/en/master/contents.html#module-scProject.rg
 Visualization | https://scproject.readthedocs.io/en/master/contents.html#module-scProject.viz
 Statistics    | https://scproject.readthedocs.io/en/master/contents.html#module-scProject.stats
 Utilities     | https://scproject.readthedocs.io/en/master/contents.html#module-scProject.matcher
 Tutorial      | https://scproject.readthedocs.io/en/master/tutorial.html
 
-## Indices and tables ##
-
-Name          | Link
-------------- | -------------
-Module Index  | https://scproject.readthedocs.io/en/master/py-modindex.html
-Search Page   | https://scproject.readthedocs.io/en/master/search.html
 
 ## Additional Information ##
 
 For more instructions and guidelines, read the [documentation](https://scproject.readthedocs.io/en/master/).  
 If you would like to leave a feedback, please contact [cshin12@jhu.edu](mailto:cshin12@jhu.edu).
```

### Comparing `scProject-stable-1.1.1/scProject_stable.egg-info/requires.txt` & `scProject-stable-1.1.2/scProject_stable.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scProject-stable-1.1.1/setup.py` & `scProject-stable-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     packages=setuptools.find_packages(),
     install_requires=requirements,
     name='scProject-stable',
-    version='1.1.1',
+    version='1.1.2',
     author='Asher Baraban, Charles Shin, Genevieve Stein-O\'Brien, Loyal Goff',
     author_email='asher.baraban@wustl.edu, cshin12@jhu.edu',
     scripts=[],
     url="https://github.com/gofflab/scProject",
     license='MIT',
     description='Transfer learning framework for single cell gene expression analysis in Python',
     long_description=open('README.md').read(),
```

