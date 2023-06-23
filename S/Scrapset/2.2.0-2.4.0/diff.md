# Comparing `tmp/Scrapset-2.2.0.tar.gz` & `tmp/Scrapset-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scrapset-2.2.0.tar", last modified: Fri Jun 23 22:14:53 2023, max compression
+gzip compressed data, was "Scrapset-2.4.0.tar", last modified: Fri Jun 23 22:25:34 2023, max compression
```

## Comparing `Scrapset-2.2.0.tar` & `Scrapset-2.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 22:14:53.725753 Scrapset-2.2.0/
--rw-rw-rw-   0        0        0     4280 2023-06-23 22:14:53.726750 Scrapset-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4049 2023-06-05 16:18:22.000000 Scrapset-2.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 22:14:53.717858 Scrapset-2.2.0/Scrapset/
--rw-rw-rw-   0        0        0     6576 2023-06-23 22:13:35.000000 Scrapset-2.2.0/Scrapset/Scrapset.py
--rw-rw-rw-   0        0        0       49 2023-06-06 18:47:28.000000 Scrapset-2.2.0/Scrapset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 22:14:53.724757 Scrapset-2.2.0/Scrapset.egg-info/
--rw-rw-rw-   0        0        0     4280 2023-06-23 22:14:53.000000 Scrapset-2.2.0/Scrapset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-23 22:14:53.000000 Scrapset-2.2.0/Scrapset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 22:14:53.000000 Scrapset-2.2.0/Scrapset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-06 18:48:01.000000 Scrapset-2.2.0/Scrapset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-06-23 22:14:53.000000 Scrapset-2.2.0/Scrapset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 22:14:53.000000 Scrapset-2.2.0/Scrapset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-2.2.0/licence.txt
--rw-rw-rw-   0        0        0      158 2023-06-23 22:14:53.726750 Scrapset-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0      499 2023-06-23 22:14:30.000000 Scrapset-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 22:25:34.464817 Scrapset-2.4.0/
+-rw-rw-rw-   0        0        0     4280 2023-06-23 22:25:34.466197 Scrapset-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4049 2023-06-05 16:18:22.000000 Scrapset-2.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 22:25:34.447986 Scrapset-2.4.0/Scrapset/
+-rw-rw-rw-   0        0        0     6580 2023-06-23 22:24:56.000000 Scrapset-2.4.0/Scrapset/Scrapset.py
+-rw-rw-rw-   0        0        0       49 2023-06-06 18:47:28.000000 Scrapset-2.4.0/Scrapset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 22:25:34.463313 Scrapset-2.4.0/Scrapset.egg-info/
+-rw-rw-rw-   0        0        0     4280 2023-06-23 22:25:34.000000 Scrapset-2.4.0/Scrapset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-23 22:25:34.000000 Scrapset-2.4.0/Scrapset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 22:25:34.000000 Scrapset-2.4.0/Scrapset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-06 18:48:01.000000 Scrapset-2.4.0/Scrapset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-06-23 22:25:34.000000 Scrapset-2.4.0/Scrapset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 22:25:34.000000 Scrapset-2.4.0/Scrapset.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-2.4.0/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-06-23 22:25:34.468199 Scrapset-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      499 2023-06-23 22:25:07.000000 Scrapset-2.4.0/setup.py
```

### Comparing `Scrapset-2.2.0/PKG-INFO` & `Scrapset-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 2.2.0
+Version: 2.4.0
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-2.2.0/README.md` & `Scrapset-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `Scrapset-2.2.0/Scrapset/Scrapset.py` & `Scrapset-2.4.0/Scrapset/Scrapset.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,20 +50,20 @@
             return list_of_dic
         except:
             logging.error("Invalid Url")
     def kaggle_discussions(self,url,initial_page,last_page):
         try:
             self.url=url
             driver=webdriver.Chrome()
-            time.sleep(1)
+            time.sleep(0.8)
             list_of_dic = {'title': [],'all_details':[],'up_vote':[],'comments':[]}  # Initialize the dictionary
             while initial_page <= last_page:
                 driver.get(url+f'/discussions?page={initial_page}')
                 initial_page=initial_page+1
-                time.sleep(2)
+                time.sleep(0.5)
                 threads=driver.find_elements(By.XPATH,'//*[@id="site-content"]/section[2]/div[2]/div/div/div/div/div[4]/ul/li/div[1]')
                 c=0
                 for thread in threads:
                     c=c+1
                     try:
                         title=thread.find_element(By.XPATH,f'//*[@id="site-content"]/section[2]/div[2]/div/div/div/div/div[4]/ul/li[{c}]/div[1]/a/div/div/div').text
                         all_details=thread.find_element(By.XPATH,f'//*[@id="site-content"]/section[2]/div[2]/div/div/div/div/div[4]/ul/li[{c}]/div[1]/a/div/span').text
```

### Comparing `Scrapset-2.2.0/Scrapset.egg-info/PKG-INFO` & `Scrapset-2.4.0/Scrapset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 2.2.0
+Version: 2.4.0
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-2.2.0/licence.txt` & `Scrapset-2.4.0/licence.txt`

 * *Files identical despite different names*

