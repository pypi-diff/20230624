# Comparing `tmp/maadstml-3.39.tar.gz` & `tmp/maadstml-3.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadstml-3.39.tar", last modified: Sat Jun 24 18:16:47 2023, max compression
+gzip compressed data, was "maadstml-3.40.tar", last modified: Sat Jun 24 19:41:00 2023, max compression
```

## Comparing `maadstml-3.39.tar` & `maadstml-3.40.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 18:16:47.249958 maadstml-3.39/
--rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.39/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.39/MANIFEST.in
--rw-rw-rw-   0        0        0   174063 2023-06-24 18:16:47.249958 maadstml-3.39/PKG-INFO
--rw-rw-rw-   0        0        0   173466 2023-06-24 18:13:52.000000 maadstml-3.39/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 18:16:47.218073 maadstml-3.39/maadstml/
--rw-rw-rw-   0        0        0     2260 2023-06-24 18:12:51.000000 maadstml-3.39/maadstml/__init__.py
--rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.39/maadstml/readpdf.py
--rw-rw-rw-   0        0        0    81197 2023-06-24 18:12:26.000000 maadstml-3.39/maadstml/sendfiles.py
--rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.39/maadstml/tmltextsummary.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:16:47.249958 maadstml-3.39/maadstml.egg-info/
--rw-rw-rw-   0        0        0   174063 2023-06-24 18:16:46.000000 maadstml-3.39/maadstml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-06-24 18:16:47.000000 maadstml-3.39/maadstml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 18:16:46.000000 maadstml-3.39/maadstml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      189 2023-06-24 18:16:46.000000 maadstml-3.39/maadstml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-24 18:16:46.000000 maadstml-3.39/maadstml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      204 2023-06-24 18:15:22.000000 maadstml-3.39/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 18:16:47.249958 maadstml-3.39/setup.cfg
--rw-rw-rw-   0        0        0     1088 2023-06-24 18:14:31.000000 maadstml-3.39/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 19:41:00.530276 maadstml-3.40/
+-rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.40/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.40/MANIFEST.in
+-rw-rw-rw-   0        0        0   173475 2023-06-24 19:41:00.530276 maadstml-3.40/PKG-INFO
+-rw-rw-rw-   0        0        0   172878 2023-06-24 19:39:52.000000 maadstml-3.40/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 19:41:00.502869 maadstml-3.40/maadstml/
+-rw-rw-rw-   0        0        0     2260 2023-06-24 18:40:37.000000 maadstml-3.40/maadstml/__init__.py
+-rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.40/maadstml/readpdf.py
+-rw-rw-rw-   0        0        0    81197 2023-06-24 18:12:26.000000 maadstml-3.40/maadstml/sendfiles.py
+-rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.40/maadstml/tmltextsummary.py
+drwxrwxrwx   0        0        0        0 2023-06-24 19:41:00.522427 maadstml-3.40/maadstml.egg-info/
+-rw-rw-rw-   0        0        0   173475 2023-06-24 19:41:00.000000 maadstml-3.40/maadstml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-06-24 19:41:00.000000 maadstml-3.40/maadstml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 19:41:00.000000 maadstml-3.40/maadstml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      189 2023-06-24 19:41:00.000000 maadstml-3.40/maadstml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-24 19:41:00.000000 maadstml-3.40/maadstml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      204 2023-06-24 18:15:22.000000 maadstml-3.40/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 19:41:00.530276 maadstml-3.40/setup.cfg
+-rw-rw-rw-   0        0        0     1088 2023-06-24 19:40:15.000000 maadstml-3.40/setup.py
```

### Comparing `maadstml-3.39/LICENSE.txt` & `maadstml-3.40/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maadstml-3.39/PKG-INFO` & `maadstml-3.40/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.39
+Version: 3.40
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
@@ -4586,36 +4586,7 @@
 
 *pdffilename,labelname,arcotype* : string, required
 
 - Acrobyte tag in PDF i.e. LTTextLineHorizontal
 
 RETURNS: Value of the labelname - if any.
 
-**40. maadstml.viperimagetotext(imagefilename)**
-
-**Parameters:**	Extract text from images.
-
-*imagefilename* : string, required
-
-- Image filename like PNG, JPG etc.
-
-RETURNS: Text in image.
-
-**41. maadstml.vipervideototext(videofilename)**
-
-**Parameters:**	Extract text from video.
-
-*videofilename* : string, required
-
-- Video filename like MP4 etc.
-
-RETURNS: Text in video.
-
-**42. maadstml.viperaudiototext(audiofilename)**
-
-**Parameters:**	Extract text from audio
-
-*audiofilename* : string, required
-
-- Audio filename like WAV etc.
-
-RETURNS: Text in audio.
```

### Comparing `maadstml-3.39/README.md` & `maadstml-3.40/maadstml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: maadstml
+Version: 3.40
+Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
+Home-page: https://github.com/smaurice101/transactionalmachinelearning
+Author: Sebastian Maurice
+Author-email: sebastian.maurice@otics.ca
+License: MIT License
+Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
+Description-Content-Type: text/markdown
+License-File: license.txt
+
 **Multi-Agent Accelerator for Data Science Using Transactional Machine Learning (MAADSTML)**
 
 *Revolutionizing Data Stream Science with Transactional Machine Learning*
 
 **Overview**
 
 *MAADSTML combines Artificial Intelligence, ChatGPT, Auto Machine Learning with Data Streams Integrated with Apache Kafka (or Redpanda) to create frictionless and elastic machine learning solutions.*  
@@ -4574,36 +4586,7 @@
 
 *pdffilename,labelname,arcotype* : string, required
 
 - Acrobyte tag in PDF i.e. LTTextLineHorizontal
 
 RETURNS: Value of the labelname - if any.
 
-**40. maadstml.viperimagetotext(imagefilename)**
-
-**Parameters:**	Extract text from images.
-
-*imagefilename* : string, required
-
-- Image filename like PNG, JPG etc.
-
-RETURNS: Text in image.
-
-**41. maadstml.vipervideototext(videofilename)**
-
-**Parameters:**	Extract text from video.
-
-*videofilename* : string, required
-
-- Video filename like MP4 etc.
-
-RETURNS: Text in video.
-
-**42. maadstml.viperaudiototext(audiofilename)**
-
-**Parameters:**	Extract text from audio
-
-*audiofilename* : string, required
-
-- Audio filename like WAV etc.
-
-RETURNS: Text in audio.
```

### Comparing `maadstml-3.39/maadstml/__init__.py` & `maadstml-3.40/maadstml/__init__.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.39/maadstml/readpdf.py` & `maadstml-3.40/maadstml/readpdf.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.39/maadstml/sendfiles.py` & `maadstml-3.40/maadstml/sendfiles.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.39/maadstml/tmltextsummary.py` & `maadstml-3.40/maadstml/tmltextsummary.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.39/maadstml.egg-info/PKG-INFO` & `maadstml-3.40/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: maadstml
-Version: 3.39
-Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
-Home-page: https://github.com/smaurice101/transactionalmachinelearning
-Author: Sebastian Maurice
-Author-email: sebastian.maurice@otics.ca
-License: MIT License
-Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
-Description-Content-Type: text/markdown
-License-File: license.txt
-
 **Multi-Agent Accelerator for Data Science Using Transactional Machine Learning (MAADSTML)**
 
 *Revolutionizing Data Stream Science with Transactional Machine Learning*
 
 **Overview**
 
 *MAADSTML combines Artificial Intelligence, ChatGPT, Auto Machine Learning with Data Streams Integrated with Apache Kafka (or Redpanda) to create frictionless and elastic machine learning solutions.*  
@@ -4586,36 +4574,7 @@
 
 *pdffilename,labelname,arcotype* : string, required
 
 - Acrobyte tag in PDF i.e. LTTextLineHorizontal
 
 RETURNS: Value of the labelname - if any.
 
-**40. maadstml.viperimagetotext(imagefilename)**
-
-**Parameters:**	Extract text from images.
-
-*imagefilename* : string, required
-
-- Image filename like PNG, JPG etc.
-
-RETURNS: Text in image.
-
-**41. maadstml.vipervideototext(videofilename)**
-
-**Parameters:**	Extract text from video.
-
-*videofilename* : string, required
-
-- Video filename like MP4 etc.
-
-RETURNS: Text in video.
-
-**42. maadstml.viperaudiototext(audiofilename)**
-
-**Parameters:**	Extract text from audio
-
-*audiofilename* : string, required
-
-- Audio filename like WAV etc.
-
-RETURNS: Text in audio.
```

### Comparing `maadstml-3.39/setup.py` & `maadstml-3.40/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maadstml',
-    version='3.39',
+    version='3.40',
     description='Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning',
     license='MIT License',
     packages=['maadstml'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
```

