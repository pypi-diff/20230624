# Comparing `tmp/ARIclicker-0.3.4.tar.gz` & `tmp/ARIclicker-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ARIclicker-0.3.4.tar", last modified: Sat Jun 24 04:11:06 2023, max compression
+gzip compressed data, was "ARIclicker-0.3.5.tar", last modified: Sat Jun 24 04:20:44 2023, max compression
```

## Comparing `ARIclicker-0.3.4.tar` & `ARIclicker-0.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 04:11:06.754696 ARIclicker-0.3.4/
-drwxrwxrwx   0        0        0        0 2023-06-24 04:11:06.723462 ARIclicker-0.3.4/ARIclicker/
--rw-rw-rw-   0        0        0     4195 2023-06-24 04:10:02.000000 ARIclicker-0.3.4/ARIclicker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 04:11:06.754696 ARIclicker-0.3.4/ARIclicker.egg-info/
--rw-rw-rw-   0        0        0     1792 2023-06-24 04:11:06.000000 ARIclicker-0.3.4/ARIclicker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-06-24 04:11:06.000000 ARIclicker-0.3.4/ARIclicker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 04:11:06.000000 ARIclicker-0.3.4/ARIclicker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-24 04:11:06.000000 ARIclicker-0.3.4/ARIclicker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 04:11:06.000000 ARIclicker-0.3.4/ARIclicker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1792 2023-06-24 04:11:06.754696 ARIclicker-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     1436 2023-06-24 04:09:50.000000 ARIclicker-0.3.4/README.md
--rw-rw-rw-   0        0        0     1093 2023-06-22 03:55:50.000000 ARIclicker-0.3.4/license.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 04:11:06.754696 ARIclicker-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      696 2023-06-24 04:10:35.000000 ARIclicker-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 04:20:44.901570 ARIclicker-0.3.5/
+drwxrwxrwx   0        0        0        0 2023-06-24 04:20:44.870348 ARIclicker-0.3.5/ARIclicker/
+-rw-rw-rw-   0        0        0     4195 2023-06-24 04:10:02.000000 ARIclicker-0.3.5/ARIclicker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 04:20:44.885958 ARIclicker-0.3.5/ARIclicker.egg-info/
+-rw-rw-rw-   0        0        0     1891 2023-06-24 04:20:44.000000 ARIclicker-0.3.5/ARIclicker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-06-24 04:20:44.000000 ARIclicker-0.3.5/ARIclicker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 04:20:44.000000 ARIclicker-0.3.5/ARIclicker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-24 04:20:44.000000 ARIclicker-0.3.5/ARIclicker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 04:20:44.000000 ARIclicker-0.3.5/ARIclicker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1891 2023-06-24 04:20:44.901570 ARIclicker-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1535 2023-06-24 04:20:24.000000 ARIclicker-0.3.5/README.md
+-rw-rw-rw-   0        0        0     1093 2023-06-22 03:55:50.000000 ARIclicker-0.3.5/license.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 04:20:44.901570 ARIclicker-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      696 2023-06-24 04:20:32.000000 ARIclicker-0.3.5/setup.py
```

### Comparing `ARIclicker-0.3.4/ARIclicker/__init__.py` & `ARIclicker-0.3.5/ARIclicker/__init__.py`

 * *Files identical despite different names*

### Comparing `ARIclicker-0.3.4/ARIclicker.egg-info/PKG-INFO` & `ARIclicker-0.3.5/ARIclicker.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 Metadata-Version: 2.1
 Name: ARIclicker
-Version: 0.3.4
+Version: 0.3.5
 Summary: AutoRandomIntervalClicker
 Home-page: UNKNOWN
 Author: lin_zhe
 Author-email: 2081812728@qq.com
 Maintainer: lin_zhe
 License: MIT License
 Keywords: AutoRandomIntervalClicker
 Platform: any
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: license.txt
 
-## How to use the ARIclicker? 
+# **How to use the ARIclicker?**
+
+## **explanation:** 
 
-**explanation:** 
 "ARIclicker" is "Auto Random Interval clicker".
 
  This is a very good autoclicker, easy to use and intelligent.
 
 
-### **First of all** 
+## **First of all** 
 
 You need to install **ARIclicker**: Open `cmd` and type `pip install ARIclicker`
 
-### Function:
 
-**syntax:**
+# **syntax:**
 
-**clicker**:
+## **clicker**:
 
 (autoclick)
 `
-ARIclicker.autoclick("start_pause_key","end_key","min_interval(sec)","max_interval(sec)","button")
+ARIclicker.autoclick(start_stop_key_character, end_key_character, button,delay_min=None, delay_max=None, delay=None)
 `
 
 (quickclick)
 `
-ARIclicker.quickclick(key_start,key_stop,program_stop_key=None)
+ARIclicker.quickclick(key_start,key_stop,program_stop_key=None,delay_min=None,delay_max=None,delay=None)
 `
 
-**presser**:
+## **presser**:
 `
 ARIclicker.autopress("start_pause_key","end_key","pressed_button")
 `
 
 example 1:
 <pre>
 	import ARIclicker 
-	ARIclicker.autoclick("a","b","0.1","1","left")
+	ARIclicker.autoclick("a","b","left",delay_min=0.1,delay_max=1)
 </pre>
 
 **explanation:** If you press the "a" key, clicking will start. When you press the "a" key again, clicking will pause. When you press the "b" key, the program will exit. The range of click intervals is between 0.1 and 1 second, and the left mouse button is the key clicked.
 
 example 2:
 <pre>
 	import ARIclicker
@@ -62,19 +62,19 @@
 
 
 **explanation:** If you press the "a" key,pressing will start.When you press the "a" key again, pressing will pause.When you press the "b" key, the program will exit.The 'c' key represents the key that will be pressed.
 
 example 3:
 <pre>
 	import ARIclicker
-	ARIclicker.quickclick("a","b")
+	ARIclicker.quickclick("a","b",delay_min=0.1,delay_max=1)
 </pre>
 
 
- ### **have fun~**
+ ## **have fun~**
```

### Comparing `ARIclicker-0.3.4/PKG-INFO` & `ARIclicker-0.3.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 Metadata-Version: 2.1
 Name: ARIclicker
-Version: 0.3.4
+Version: 0.3.5
 Summary: AutoRandomIntervalClicker
 Home-page: UNKNOWN
 Author: lin_zhe
 Author-email: 2081812728@qq.com
 Maintainer: lin_zhe
 License: MIT License
 Keywords: AutoRandomIntervalClicker
 Platform: any
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: license.txt
 
-## How to use the ARIclicker? 
+# **How to use the ARIclicker?**
+
+## **explanation:** 
 
-**explanation:** 
 "ARIclicker" is "Auto Random Interval clicker".
 
  This is a very good autoclicker, easy to use and intelligent.
 
 
-### **First of all** 
+## **First of all** 
 
 You need to install **ARIclicker**: Open `cmd` and type `pip install ARIclicker`
 
-### Function:
 
-**syntax:**
+# **syntax:**
 
-**clicker**:
+## **clicker**:
 
 (autoclick)
 `
-ARIclicker.autoclick("start_pause_key","end_key","min_interval(sec)","max_interval(sec)","button")
+ARIclicker.autoclick(start_stop_key_character, end_key_character, button,delay_min=None, delay_max=None, delay=None)
 `
 
 (quickclick)
 `
-ARIclicker.quickclick(key_start,key_stop,program_stop_key=None)
+ARIclicker.quickclick(key_start,key_stop,program_stop_key=None,delay_min=None,delay_max=None,delay=None)
 `
 
-**presser**:
+## **presser**:
 `
 ARIclicker.autopress("start_pause_key","end_key","pressed_button")
 `
 
 example 1:
 <pre>
 	import ARIclicker 
-	ARIclicker.autoclick("a","b","0.1","1","left")
+	ARIclicker.autoclick("a","b","left",delay_min=0.1,delay_max=1)
 </pre>
 
 **explanation:** If you press the "a" key, clicking will start. When you press the "a" key again, clicking will pause. When you press the "b" key, the program will exit. The range of click intervals is between 0.1 and 1 second, and the left mouse button is the key clicked.
 
 example 2:
 <pre>
 	import ARIclicker
@@ -62,19 +62,19 @@
 
 
 **explanation:** If you press the "a" key,pressing will start.When you press the "a" key again, pressing will pause.When you press the "b" key, the program will exit.The 'c' key represents the key that will be pressed.
 
 example 3:
 <pre>
 	import ARIclicker
-	ARIclicker.quickclick("a","b")
+	ARIclicker.quickclick("a","b",delay_min=0.1,delay_max=1)
 </pre>
 
 
- ### **have fun~**
+ ## **have fun~**
```

### Comparing `ARIclicker-0.3.4/README.md` & `ARIclicker-0.3.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-## How to use the ARIclicker? 
+# **How to use the ARIclicker?**
+
+## **explanation:** 
 
-**explanation:** 
 "ARIclicker" is "Auto Random Interval clicker".
 
  This is a very good autoclicker, easy to use and intelligent.
 
 
-### **First of all** 
+## **First of all** 
 
 You need to install **ARIclicker**: Open `cmd` and type `pip install ARIclicker`
 
-### Function:
 
-**syntax:**
+# **syntax:**
 
-**clicker**:
+## **clicker**:
 
 (autoclick)
 `
-ARIclicker.autoclick("start_pause_key","end_key","min_interval(sec)","max_interval(sec)","button")
+ARIclicker.autoclick(start_stop_key_character, end_key_character, button,delay_min=None, delay_max=None, delay=None)
 `
 
 (quickclick)
 `
-ARIclicker.quickclick(key_start,key_stop,program_stop_key=None)
+ARIclicker.quickclick(key_start,key_stop,program_stop_key=None,delay_min=None,delay_max=None,delay=None)
 `
 
-**presser**:
+## **presser**:
 `
 ARIclicker.autopress("start_pause_key","end_key","pressed_button")
 `
 
 example 1:
 <pre>
 	import ARIclicker 
-	ARIclicker.autoclick("a","b","0.1","1","left")
+	ARIclicker.autoclick("a","b","left",delay_min=0.1,delay_max=1)
 </pre>
 
 **explanation:** If you press the "a" key, clicking will start. When you press the "a" key again, clicking will pause. When you press the "b" key, the program will exit. The range of click intervals is between 0.1 and 1 second, and the left mouse button is the key clicked.
 
 example 2:
 <pre>
 	import ARIclicker
@@ -47,19 +47,19 @@
 
 
 **explanation:** If you press the "a" key,pressing will start.When you press the "a" key again, pressing will pause.When you press the "b" key, the program will exit.The 'c' key represents the key that will be pressed.
 
 example 3:
 <pre>
 	import ARIclicker
-	ARIclicker.quickclick("a","b")
+	ARIclicker.quickclick("a","b",delay_min=0.1,delay_max=1)
 </pre>
 
 
- ### **have fun~**
+ ## **have fun~**
```

### Comparing `ARIclicker-0.3.4/license.txt` & `ARIclicker-0.3.5/license.txt`

 * *Files identical despite different names*

### Comparing `ARIclicker-0.3.4/setup.py` & `ARIclicker-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setup(
     name = 'ARIclicker',
-    version = '0.3.4',
+    version = '0.3.5',
     maintainer='lin_zhe',
     keywords='AutoRandomIntervalClicker',
     description = 'AutoRandomIntervalClicker',
     long_description_content_type='text/markdown',
     long_description=long_description,
     license = 'MIT License',
     author = 'lin_zhe',
```

