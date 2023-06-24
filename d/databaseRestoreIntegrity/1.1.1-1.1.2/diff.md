# Comparing `tmp/databaseRestoreIntegrity-1.1.1.tar.gz` & `tmp/databaseRestoreIntegrity-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databaseRestoreIntegrity-1.1.1.tar", last modified: Fri Jun 23 11:50:13 2023, max compression
+gzip compressed data, was "databaseRestoreIntegrity-1.1.2.tar", last modified: Sat Jun 24 16:15:19 2023, max compression
```

## Comparing `databaseRestoreIntegrity-1.1.1.tar` & `databaseRestoreIntegrity-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-23 11:50:13.750264 databaseRestoreIntegrity-1.1.1/
--rw-r--r--   0 mhasan     (502) staff       (20)     1073 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.1.1/LICENSE.txt
--rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.1.1/MANIFEST.in
--rw-r--r--   0 mhasan     (502) staff       (20)     6231 2023-06-23 11:50:13.750347 databaseRestoreIntegrity-1.1.1/PKG-INFO
--rw-r--r--   0 mhasan     (502) staff       (20)     4539 2023-06-23 10:14:38.000000 databaseRestoreIntegrity-1.1.1/README.md
--rw-r--r--   0 mhasan     (502) staff       (20)       84 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.1.1/pyproject.toml
--rw-r--r--   0 mhasan     (502) staff       (20)      740 2023-06-23 11:50:13.751241 databaseRestoreIntegrity-1.1.1/setup.cfg
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-23 11:50:13.738617 databaseRestoreIntegrity-1.1.1/src/
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-23 11:50:13.746968 databaseRestoreIntegrity-1.1.1/src/databaseRestoreIntegrity/
--rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.1.1/src/databaseRestoreIntegrity/__init__.py
--rw-r--r--   0 mhasan     (502) staff       (20)     3149 2023-06-23 11:49:26.000000 databaseRestoreIntegrity-1.1.1/src/databaseRestoreIntegrity/mysqldb.py
--rw-r--r--   0 mhasan     (502) staff       (20)     2872 2023-06-15 13:02:54.000000 databaseRestoreIntegrity-1.1.1/src/databaseRestoreIntegrity/postgresdb.py
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-23 11:50:13.749910 databaseRestoreIntegrity-1.1.1/src/databaseRestoreIntegrity.egg-info/
--rw-r--r--   0 mhasan     (502) staff       (20)     6231 2023-06-23 11:50:13.000000 databaseRestoreIntegrity-1.1.1/src/databaseRestoreIntegrity.egg-info/PKG-INFO
--rw-r--r--   0 mhasan     (502) staff       (20)      390 2023-06-23 11:50:13.000000 databaseRestoreIntegrity-1.1.1/src/databaseRestoreIntegrity.egg-info/SOURCES.txt
--rw-r--r--   0 mhasan     (502) staff       (20)        1 2023-06-23 11:50:13.000000 databaseRestoreIntegrity-1.1.1/src/databaseRestoreIntegrity.egg-info/dependency_links.txt
--rw-r--r--   0 mhasan     (502) staff       (20)       25 2023-06-23 11:50:13.000000 databaseRestoreIntegrity-1.1.1/src/databaseRestoreIntegrity.egg-info/top_level.txt
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-24 16:15:19.481331 databaseRestoreIntegrity-1.1.2/
+-rw-r--r--   0 mhasan     (502) staff       (20)     1073 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.1.2/LICENSE.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.1.2/MANIFEST.in
+-rw-r--r--   0 mhasan     (502) staff       (20)     6231 2023-06-24 16:15:19.481459 databaseRestoreIntegrity-1.1.2/PKG-INFO
+-rw-r--r--   0 mhasan     (502) staff       (20)     4539 2023-06-23 10:14:38.000000 databaseRestoreIntegrity-1.1.2/README.md
+-rw-r--r--   0 mhasan     (502) staff       (20)       84 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.1.2/pyproject.toml
+-rw-r--r--   0 mhasan     (502) staff       (20)      740 2023-06-24 16:15:19.482595 databaseRestoreIntegrity-1.1.2/setup.cfg
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-24 16:15:19.467876 databaseRestoreIntegrity-1.1.2/src/
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-24 16:15:19.476359 databaseRestoreIntegrity-1.1.2/src/databaseRestoreIntegrity/
+-rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.1.2/src/databaseRestoreIntegrity/__init__.py
+-rw-r--r--   0 mhasan     (502) staff       (20)     3289 2023-06-24 16:11:27.000000 databaseRestoreIntegrity-1.1.2/src/databaseRestoreIntegrity/mysqldb.py
+-rw-r--r--   0 mhasan     (502) staff       (20)     2872 2023-06-15 13:02:54.000000 databaseRestoreIntegrity-1.1.2/src/databaseRestoreIntegrity/postgresdb.py
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-24 16:15:19.480892 databaseRestoreIntegrity-1.1.2/src/databaseRestoreIntegrity.egg-info/
+-rw-r--r--   0 mhasan     (502) staff       (20)     6231 2023-06-24 16:15:19.000000 databaseRestoreIntegrity-1.1.2/src/databaseRestoreIntegrity.egg-info/PKG-INFO
+-rw-r--r--   0 mhasan     (502) staff       (20)      390 2023-06-24 16:15:19.000000 databaseRestoreIntegrity-1.1.2/src/databaseRestoreIntegrity.egg-info/SOURCES.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)        1 2023-06-24 16:15:19.000000 databaseRestoreIntegrity-1.1.2/src/databaseRestoreIntegrity.egg-info/dependency_links.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)       25 2023-06-24 16:15:19.000000 databaseRestoreIntegrity-1.1.2/src/databaseRestoreIntegrity.egg-info/top_level.txt
```

### Comparing `databaseRestoreIntegrity-1.1.1/LICENSE.txt` & `databaseRestoreIntegrity-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.1.1/PKG-INFO` & `databaseRestoreIntegrity-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databaseRestoreIntegrity
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package to check mysql restore integrity check
 Home-page: 
 Author: Maihraj Hasan
 Author-email: maihrajhasan@gmail.com
 Project-URL: Bug Tracker, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck/-/issues
 Project-URL: repository, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck
 Classifier: Programming Language :: Python :: 3
```

### Comparing `databaseRestoreIntegrity-1.1.1/README.md` & `databaseRestoreIntegrity-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.1.1/setup.cfg` & `databaseRestoreIntegrity-1.1.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = databaseRestoreIntegrity
-version = 1.1.1
+version = 1.1.2
 author = Maihraj Hasan
 author_email = maihrajhasan@gmail.com
 description = A package to check mysql restore integrity check
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = 
 project_urls =
```

### Comparing `databaseRestoreIntegrity-1.1.1/src/databaseRestoreIntegrity/mysqldb.py` & `databaseRestoreIntegrity-1.1.2/src/databaseRestoreIntegrity/mysqldb.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,24 +55,27 @@
         conn = self.connection()
         t_name = self._table_list()
         for c in t_name:
             ignore_dbs = ['performance_schema', 'information_schema', 'sys', 'mysql']
             if any(db in c for db in ignore_dbs):
                 pass
             else:
-                sql_query = "select count(*) from " + c
-            r = conn.cursor()
-            r.execute(sql_query)
-            for count in r:
-                records_count.append("{},{}".format(c, *count))  
+                sql_query = ("{}{}".format('select count(*) from ', c))
+                print(sql_query)
+                r = conn.cursor()
+                r.execute(sql_query)
+                for count in r:
+                    print("{}{},{}".format('---', c, *count))
+                    records_count.append("{},{}".format(c, *count))  
         return records_count   
 
     def _create_tmp_file(self, name):
         self.name = name
         records = self._records_count()
+        print
         f = open(self.name, 'w+')
         for data in records:
             sql_query = ("{}{}{}{}".format('INSERT INTO ', self.name, ' (tables_name, records_count, hostname) VALUES ', (data.split(",")[0], data.split(",")[1], self.host)))
             f.write("{}\n".format(sql_query))
         f.close()
         
     def _insert_data(self, name):
@@ -90,8 +93,8 @@
         for line in lines:
             count += 1
             sql_query = ("{}".format(line.strip()))
             ct.execute(sql_query)
             conn.commit()
         f.close()
         os.remove(self.name)
-        conn.close()
+        conn.close()
```

### Comparing `databaseRestoreIntegrity-1.1.1/src/databaseRestoreIntegrity/postgresdb.py` & `databaseRestoreIntegrity-1.1.2/src/databaseRestoreIntegrity/postgresdb.py`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.1.1/src/databaseRestoreIntegrity.egg-info/PKG-INFO` & `databaseRestoreIntegrity-1.1.2/src/databaseRestoreIntegrity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databaseRestoreIntegrity
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package to check mysql restore integrity check
 Home-page: 
 Author: Maihraj Hasan
 Author-email: maihrajhasan@gmail.com
 Project-URL: Bug Tracker, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck/-/issues
 Project-URL: repository, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck
 Classifier: Programming Language :: Python :: 3
```

