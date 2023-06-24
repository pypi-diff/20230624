# Comparing `tmp/maadstmlmedia-1.1.tar.gz` & `tmp/maadstmlmedia-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadstmlmedia-1.1.tar", last modified: Sat Jun 24 18:52:37 2023, max compression
+gzip compressed data, was "maadstmlmedia-1.2.tar", last modified: Sat Jun 24 19:31:14 2023, max compression
```

## Comparing `maadstmlmedia-1.1.tar` & `maadstmlmedia-1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 18:52:37.256264 maadstmlmedia-1.1/
--rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstmlmedia-1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstmlmedia-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2272 2023-06-24 18:52:37.256264 maadstmlmedia-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1649 2023-06-24 18:41:20.000000 maadstmlmedia-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 18:52:37.223650 maadstmlmedia-1.1/maadstmlmedia/
--rw-rw-rw-   0        0        0      157 2023-06-24 18:51:54.000000 maadstmlmedia-1.1/maadstmlmedia/__init__.py
--rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstmlmedia-1.1/maadstmlmedia/readpdf.py
--rw-rw-rw-   0        0        0     1609 2023-06-24 18:49:59.000000 maadstmlmedia-1.1/maadstmlmedia/sendfiles.py
--rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstmlmedia-1.1/maadstmlmedia/tmltextsummary.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:52:37.256264 maadstmlmedia-1.1/maadstmlmedia.egg-info/
--rw-rw-rw-   0        0        0     2272 2023-06-24 18:52:37.000000 maadstmlmedia-1.1/maadstmlmedia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-06-24 18:52:37.000000 maadstmlmedia-1.1/maadstmlmedia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 18:52:37.000000 maadstmlmedia-1.1/maadstmlmedia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      189 2023-06-24 18:52:37.000000 maadstmlmedia-1.1/maadstmlmedia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-24 18:52:37.000000 maadstmlmedia-1.1/maadstmlmedia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      204 2023-06-24 18:15:22.000000 maadstmlmedia-1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 18:52:37.256264 maadstmlmedia-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1119 2023-06-24 18:43:01.000000 maadstmlmedia-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 19:31:14.081625 maadstmlmedia-1.2/
+-rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstmlmedia-1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstmlmedia-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2272 2023-06-24 19:31:14.081625 maadstmlmedia-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1649 2023-06-24 18:41:20.000000 maadstmlmedia-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 19:31:14.063226 maadstmlmedia-1.2/maadstmlmedia/
+-rw-rw-rw-   0        0        0      157 2023-06-24 18:51:54.000000 maadstmlmedia-1.2/maadstmlmedia/__init__.py
+-rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstmlmedia-1.2/maadstmlmedia/readpdf.py
+-rw-rw-rw-   0        0        0     1609 2023-06-24 18:49:59.000000 maadstmlmedia-1.2/maadstmlmedia/sendfiles.py
+-rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstmlmedia-1.2/maadstmlmedia/tmltextsummary.py
+drwxrwxrwx   0        0        0        0 2023-06-24 19:31:14.081076 maadstmlmedia-1.2/maadstmlmedia.egg-info/
+-rw-rw-rw-   0        0        0     2272 2023-06-24 19:31:13.000000 maadstmlmedia-1.2/maadstmlmedia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-06-24 19:31:13.000000 maadstmlmedia-1.2/maadstmlmedia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 19:31:13.000000 maadstmlmedia-1.2/maadstmlmedia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-24 19:31:13.000000 maadstmlmedia-1.2/maadstmlmedia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-24 19:31:13.000000 maadstmlmedia-1.2/maadstmlmedia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       36 2023-06-24 19:30:35.000000 maadstmlmedia-1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 19:31:14.081625 maadstmlmedia-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1119 2023-06-24 19:30:58.000000 maadstmlmedia-1.2/setup.py
```

### Comparing `maadstmlmedia-1.1/LICENSE.txt` & `maadstmlmedia-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maadstmlmedia-1.1/PKG-INFO` & `maadstmlmedia-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstmlmedia
-Version: 1.1
+Version: 1.2
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, audio, video, images, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
```

### Comparing `maadstmlmedia-1.1/README.md` & `maadstmlmedia-1.2/README.md`

 * *Files identical despite different names*

### Comparing `maadstmlmedia-1.1/maadstmlmedia/readpdf.py` & `maadstmlmedia-1.2/maadstmlmedia/readpdf.py`

 * *Files identical despite different names*

### Comparing `maadstmlmedia-1.1/maadstmlmedia/sendfiles.py` & `maadstmlmedia-1.2/maadstmlmedia/sendfiles.py`

 * *Files identical despite different names*

### Comparing `maadstmlmedia-1.1/maadstmlmedia/tmltextsummary.py` & `maadstmlmedia-1.2/maadstmlmedia/tmltextsummary.py`

 * *Files identical despite different names*

### Comparing `maadstmlmedia-1.1/maadstmlmedia.egg-info/PKG-INFO` & `maadstmlmedia-1.2/maadstmlmedia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstmlmedia
-Version: 1.1
+Version: 1.2
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, audio, video, images, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
```

### Comparing `maadstmlmedia-1.1/setup.py` & `maadstmlmedia-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maadstmlmedia',
-    version='1.1',
+    version='1.2',
     description='Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning',
     license='MIT License',
     packages=['maadstmlmedia'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, transactional machine learning, audio, video, images, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
```

