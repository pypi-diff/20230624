# Comparing `tmp/prophecy_spark_ai-0.1.6-py3-none-any.whl.zip` & `tmp/prophecy_spark_ai-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 10220 bytes, number of entries: 15
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 05:52 spark_ai/__init__.py
--rw-r--r--  2.0 unx     3790 b- defN 23-Jun-17 19:34 spark_ai/spark.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-11 01:22 spark_ai/dbs/__init__.py
--rw-r--r--  2.0 unx     2241 b- defN 23-Jun-20 16:59 spark_ai/dbs/pinecone.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 01:21 spark_ai/files/__init__.py
--rw-r--r--  2.0 unx     1049 b- defN 23-Jun-13 01:29 spark_ai/files/pdf.py
--rw-r--r--  2.0 unx      513 b- defN 23-Jun-13 01:26 spark_ai/files/text.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-10 01:44 spark_ai/llms/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 23-Jun-17 19:34 spark_ai/llms/openai.py
--rw-r--r--  2.0 unx      677 b- defN 23-Jun-15 03:40 spark_ai/webapps/__init__.py
--rw-r--r--  2.0 unx     9643 b- defN 23-Jun-20 05:31 spark_ai/webapps/slack.py
--rw-r--r--  2.0 unx     3603 b- defN 23-Jun-20 20:41 prophecy_spark_ai-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 20:41 prophecy_spark_ai-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-20 20:41 prophecy_spark_ai-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1205 b- defN 23-Jun-20 20:41 prophecy_spark_ai-0.1.6.dist-info/RECORD
-15 files, 25568 bytes uncompressed, 8212 bytes compressed:  67.9%
+Zip file size: 10232 bytes, number of entries: 15
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 06:15 spark_ai/__init__.py
+-rw-r--r--  2.0 unx     3790 b- defN 23-Jun-21 06:15 spark_ai/spark.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 06:15 spark_ai/dbs/__init__.py
+-rw-r--r--  2.0 unx     2241 b- defN 23-Jun-21 06:15 spark_ai/dbs/pinecone.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 06:15 spark_ai/files/__init__.py
+-rw-r--r--  2.0 unx     1049 b- defN 23-Jun-21 06:15 spark_ai/files/pdf.py
+-rw-r--r--  2.0 unx      513 b- defN 23-Jun-21 06:15 spark_ai/files/text.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 06:15 spark_ai/llms/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 23-Jun-21 06:15 spark_ai/llms/openai.py
+-rw-r--r--  2.0 unx      689 b- defN 23-Jun-22 23:34 spark_ai/webapps/__init__.py
+-rw-r--r--  2.0 unx     9643 b- defN 23-Jun-21 06:15 spark_ai/webapps/slack.py
+-rw-r--r--  2.0 unx     3603 b- defN 23-Jun-24 18:53 prophecy_spark_ai-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 18:53 prophecy_spark_ai-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-24 18:53 prophecy_spark_ai-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1205 b- defN 23-Jun-24 18:53 prophecy_spark_ai-0.1.7.dist-info/RECORD
+15 files, 25580 bytes uncompressed, 8224 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: spark_ai/webapps/__init__.py
 Comment: 
 
 Filename: spark_ai/webapps/slack.py
 Comment: 
 
-Filename: prophecy_spark_ai-0.1.6.dist-info/METADATA
+Filename: prophecy_spark_ai-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: prophecy_spark_ai-0.1.6.dist-info/WHEEL
+Filename: prophecy_spark_ai-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: prophecy_spark_ai-0.1.6.dist-info/top_level.txt
+Filename: prophecy_spark_ai-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: prophecy_spark_ai-0.1.6.dist-info/RECORD
+Filename: prophecy_spark_ai-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spark_ai/webapps/__init__.py

```diff
@@ -1,17 +1,17 @@
 import requests
 from bs4 import BeautifulSoup
 from pyspark.sql import SparkSession
-from pyspark.sql.types import StringType
+from pyspark.sql.types import StringType, BinaryType
 
 
 class WebUtils:
 
     def register_udfs(self, spark: SparkSession):
-        spark.udf.register('web_scrape', self.scrape, returnType=StringType())
+        spark.udf.register('web_scrape', self.scrape, returnType=BinaryType())
         spark.udf.register('web_scrape_text', self.scrape_text, returnType=StringType())
 
     @staticmethod
     def scrape(url: str):
         response = requests.get(url)
 
         return response.content
```

## Comparing `prophecy_spark_ai-0.1.6.dist-info/METADATA` & `prophecy_spark_ai-0.1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-spark-ai
-Version: 0.1.6
+Version: 0.1.7
 Summary: High-performance AI/ML library for Spark to build and deploy your LLM applications in production.
 Home-page: https://github.com/prophecy-io/spark-ai
 Keywords: python,prophecy
 Description-Content-Type: text/markdown
 Requires-Dist: slack-sdk (>=3.21.3)
 Requires-Dist: openai[datalib] (>=0.27.8)
 Requires-Dist: pinecone-client (>=2.2.2)
```

## Comparing `prophecy_spark_ai-0.1.6.dist-info/RECORD` & `prophecy_spark_ai-0.1.7.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 spark_ai/dbs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 spark_ai/dbs/pinecone.py,sha256=qRXL4w7wLXKENiMB-ODozpfQ14uSUA034JP8OzLiEYA,2241
 spark_ai/files/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 spark_ai/files/pdf.py,sha256=_xLoM9NJ3b_Xln0Y0qFZ4JYDOlmnDofUxQQEl8FxmN8,1049
 spark_ai/files/text.py,sha256=UIb9kVsouB-bXtjb823oh2z1mDXUwR8qnMnbuBzQIzM,513
 spark_ai/llms/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 spark_ai/llms/openai.py,sha256=e55mYL8l1SHKsX-AY1DKkhutk5d9yeaOJALsQ-CwUgQ,2746
-spark_ai/webapps/__init__.py,sha256=HSUuh4DRG189E15BrYnh1bs1hym_hhkC-1_xFke0FJA,677
+spark_ai/webapps/__init__.py,sha256=cxeMGWd3705XuYVs0qez_MLfJboRLAgiK0_Lg7ULHJ8,689
 spark_ai/webapps/slack.py,sha256=k-yG3EyTZc8-gvXJaDMRnMNzCOkgeH4BYYIqZPi9x88,9643
-prophecy_spark_ai-0.1.6.dist-info/METADATA,sha256=oLE5N9XuEVykwFi_jqmik3u8pscmIJuLFAgWTwF7rgg,3603
-prophecy_spark_ai-0.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-prophecy_spark_ai-0.1.6.dist-info/top_level.txt,sha256=uriwjszTLG2ldv6q-y4J72iKjOjTn2hIFC2lcPsQBvw,9
-prophecy_spark_ai-0.1.6.dist-info/RECORD,,
+prophecy_spark_ai-0.1.7.dist-info/METADATA,sha256=NA3unu-4y_JFIkV3fSc0G5JkXpLJbewFh_GDBuI8nqQ,3603
+prophecy_spark_ai-0.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+prophecy_spark_ai-0.1.7.dist-info/top_level.txt,sha256=uriwjszTLG2ldv6q-y4J72iKjOjTn2hIFC2lcPsQBvw,9
+prophecy_spark_ai-0.1.7.dist-info/RECORD,,
```

