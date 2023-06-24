# Comparing `tmp/pyweb_db-1.0.1.tar.gz` & `tmp/pyweb_db-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweb_db-1.0.1.tar", last modified: Sat Jun 24 13:43:22 2023, max compression
+gzip compressed data, was "pyweb_db-1.0.2.tar", last modified: Sat Jun 24 17:06:07 2023, max compression
```

## Comparing `pyweb_db-1.0.1.tar` & `pyweb_db-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 13:43:22.269468 pyweb_db-1.0.1/
--rw-rw-rw-   0        0        0     1059 2023-06-24 13:11:04.000000 pyweb_db-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1895 2023-06-24 13:43:22.269468 pyweb_db-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1448 2023-06-24 13:41:47.000000 pyweb_db-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 13:43:22.236423 pyweb_db-1.0.1/pyweb_db/
--rw-rw-rw-   0        0        0     6537 2023-06-24 12:51:12.000000 pyweb_db-1.0.1/pyweb_db/__init__.py
--rw-rw-rw-   0        0        0     4383 2023-06-24 13:43:14.000000 pyweb_db-1.0.1/pyweb_db/main.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:43:22.268468 pyweb_db-1.0.1/pyweb_db.egg-info/
--rw-rw-rw-   0        0        0     1895 2023-06-24 13:43:22.000000 pyweb_db-1.0.1/pyweb_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-24 13:43:22.000000 pyweb_db-1.0.1/pyweb_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 13:43:22.000000 pyweb_db-1.0.1/pyweb_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-24 13:43:22.000000 pyweb_db-1.0.1/pyweb_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-24 13:43:22.000000 pyweb_db-1.0.1/pyweb_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2023-06-24 13:43:22.278612 pyweb_db-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      668 2023-06-24 13:41:35.000000 pyweb_db-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:06:07.137228 pyweb_db-1.0.2/
+-rw-rw-rw-   0        0        0     1059 2023-06-24 13:11:04.000000 pyweb_db-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1895 2023-06-24 17:06:07.137228 pyweb_db-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1448 2023-06-24 13:41:47.000000 pyweb_db-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 17:06:07.094624 pyweb_db-1.0.2/pyweb_db/
+-rw-rw-rw-   0        0        0     7874 2023-06-24 17:01:00.000000 pyweb_db-1.0.2/pyweb_db/__init__.py
+-rw-rw-rw-   0        0        0     4707 2023-06-24 17:04:39.000000 pyweb_db-1.0.2/pyweb_db/main.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:06:07.135253 pyweb_db-1.0.2/pyweb_db.egg-info/
+-rw-rw-rw-   0        0        0     1895 2023-06-24 17:06:06.000000 pyweb_db-1.0.2/pyweb_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-24 17:06:06.000000 pyweb_db-1.0.2/pyweb_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 17:06:06.000000 pyweb_db-1.0.2/pyweb_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-24 17:06:06.000000 pyweb_db-1.0.2/pyweb_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-24 17:06:06.000000 pyweb_db-1.0.2/pyweb_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2023-06-24 17:06:07.140253 pyweb_db-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      686 2023-06-24 17:05:21.000000 pyweb_db-1.0.2/setup.py
```

### Comparing `pyweb_db-1.0.1/LICENSE` & `pyweb_db-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyweb_db-1.0.1/PKG-INFO` & `pyweb_db-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweb_db
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is a simple JSON-based database library
 Author: PyWebSol
 Author-email: pywebsol@gmail.com
 Keywords: database python json pywebsol
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyweb_db-1.0.1/README.md` & `pyweb_db-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyweb_db-1.0.1/pyweb_db/__init__.py` & `pyweb_db-1.0.2/pyweb_db/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,21 @@
             await file.write(json.dumps(data))
     
     async def create_table(self, table_name: str):
         db_content = await self.load_data()
         if table_name not in db_content:
             db_content[table_name] = []
             await self.save_data(db_content)
+    
+    async def create_tables(self, table_names: list):
+        db_content = await self.load_data()
+        for table_name in table_names:
+            if table_name not in db_content:
+                db_content[table_name] = []
+                await self.save_data(db_content)
 
     async def insert_into_table(self, table_name: str, data, unique: bool = False):
         db_content = await self.load_data()
         if table_name in db_content:
             if (not data in db_content[table_name] and unique == True):
                 db_content[table_name].append(data)
                 await self.save_data(db_content)
@@ -59,14 +66,21 @@
     
     async def delete_table(self, table_name: str):
         db_content = await self.load_data()
         if table_name in db_content:
             del db_content[table_name]
             await self.save_data(db_content)
     
+    async def delete_tables(self, table_names: list):
+        db_content = await self.load_data()
+        for table_name in table_names:
+            if table_name in db_content:
+                del db_content[table_name]
+                await self.save_data(db_content)
+    
     async def update_data(self, table_name: str, data, replace_data):
         db_content = await self.load_data()
         if table_name in db_content and data in db_content[table_name]:
             index4replace = db_content[table_name].index(data)
             db_content[table_name][index4replace] = replace_data
             await self.save_data(db_content)
     
@@ -89,14 +103,23 @@
     def create_table(self, table_name: str):
         with open(self.path, 'r+') as file:
             db_content = json.load(file)
             if table_name not in db_content:
                 db_content[table_name] = []
                 file.seek(0)
                 json.dump(db_content, file)
+    
+    def create_tables(self, table_names: list):
+        with open(self.path, 'r+') as file:
+            db_content = json.load(file)
+            for table_name in table_names:
+                if table_name not in db_content:
+                    db_content[table_name] = []
+                    file.seek(0)
+                    json.dump(db_content, file)
 
     def insert_into_table(self, table_name: str, data, unique: bool = False):
         with open(self.path, 'r+') as file:
             db_content = json.load(file)
             if table_name in db_content:
                 if (not data in db_content[table_name] and unique == True):
                     db_content[table_name].append(data)
@@ -136,14 +159,24 @@
             db_content = json.load(file)
             if table_name in db_content:
                 del db_content[table_name]
                 file.seek(0)
                 json.dump(db_content, file)
                 file.truncate()
     
+    def delete_tables(self, table_names: list):
+        with open(self.path, 'r+') as file:
+            db_content = json.load(file)
+            for table_name in table_names:
+                if table_name in db_content:
+                    del db_content[table_name]
+                    file.seek(0)
+                    json.dump(db_content, file)
+                    file.truncate()
+    
     def update_data(self, table_name: str, data, replace_data):
         with open(self.path, 'r+') as file:
             db_content = json.load(file)
             if table_name in db_content and data in db_content[table_name]:
                 index4replace = db_content[table_name].index(data)
                 db_content[table_name][index4replace] = replace_data
                 file.seek(0)
```

### Comparing `pyweb_db-1.0.1/pyweb_db/main.py` & `pyweb_db-1.0.2/pyweb_db/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     for name, uid in zip(await conn.get_data('names'), await conn.get_data('uids')):  # Iterate over the updated data in both tables
         print(f'{name} - {uid}')  # Print the name and UID
     
     print()
     
     await conn.delete_table('uids')  # Delete the 'uids' table
     await conn.delete_table('names')  # Delete the 'names' table
+    await conn.create_tables(['test1', 'test2', 'test3']) # Create multiple tables
+    await conn.delete_tables(['test1', 'test2', 'test3']) # Delete multiple tables
 
 asyncio.run(main())  # Run the async example
 
 # sync example
 def sync_main():
     conn = pyweb_db.connection('database') # Create connection
     
@@ -81,9 +83,11 @@
     for name, uid in zip(conn.get_data('names'), conn.get_data('uids')):  # Iterate over the updated data in both tables
         print(f'{name} - {uid}')  # Print the name and UID
     
     print()
     
     conn.delete_table('uids')  # Delete the 'uids' table
     conn.delete_table('names')  # Delete the 'names' table
+    conn.create_tables(['test1', 'test2', 'test3']) # Create multiple tables
+    conn.delete_tables(['test1', 'test2', 'test3']) # Delete multiple tables
 
 sync_main()  # Run the sync example
```

### Comparing `pyweb_db-1.0.1/pyweb_db.egg-info/PKG-INFO` & `pyweb_db-1.0.2/pyweb_db.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweb-db
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is a simple JSON-based database library
 Author: PyWebSol
 Author-email: pywebsol@gmail.com
 Keywords: database python json pywebsol
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyweb_db-1.0.1/setup.py` & `pyweb_db-1.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 def readme():
-  with open('README.md', 'r') as f:
+  with open('README.md', 'r', encoding='utf-8') as f:
     return f.read()
 
 setup(
   name='pyweb_db',
-  version='1.0.1',
+  version='1.0.2',
   author='PyWebSol',
   author_email='pywebsol@gmail.com',
   description='This is a simple JSON-based database library',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
   install_requires=['aiofiles'],
```

