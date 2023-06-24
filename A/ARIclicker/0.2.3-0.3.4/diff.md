# Comparing `tmp/ARIclicker-0.2.3.tar.gz` & `tmp/ARIclicker-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ARIclicker-0.2.3.tar", last modified: Fri Jun 23 09:51:39 2023, max compression
+gzip compressed data, was "ARIclicker-0.3.4.tar", last modified: Sat Jun 24 04:11:06 2023, max compression
```

## Comparing `ARIclicker-0.2.3.tar` & `ARIclicker-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 09:51:39.724124 ARIclicker-0.2.3/
-drwxrwxrwx   0        0        0        0 2023-06-23 09:51:39.677268 ARIclicker-0.2.3/ARIclicker/
--rw-rw-rw-   0        0        0     3790 2023-06-23 09:51:28.000000 ARIclicker-0.2.3/ARIclicker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:51:39.724124 ARIclicker-0.2.3/ARIclicker.egg-info/
--rw-rw-rw-   0        0        0     1601 2023-06-23 09:51:39.000000 ARIclicker-0.2.3/ARIclicker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-06-23 09:51:39.000000 ARIclicker-0.2.3/ARIclicker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 09:51:39.000000 ARIclicker-0.2.3/ARIclicker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-23 09:51:39.000000 ARIclicker-0.2.3/ARIclicker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-23 09:51:39.000000 ARIclicker-0.2.3/ARIclicker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1601 2023-06-23 09:51:39.724124 ARIclicker-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1245 2023-06-22 04:08:21.000000 ARIclicker-0.2.3/README.md
--rw-rw-rw-   0        0        0     1093 2023-06-22 03:55:50.000000 ARIclicker-0.2.3/license.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 09:51:39.724124 ARIclicker-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      696 2023-06-23 09:51:20.000000 ARIclicker-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 04:11:06.754696 ARIclicker-0.3.4/
+drwxrwxrwx   0        0        0        0 2023-06-24 04:11:06.723462 ARIclicker-0.3.4/ARIclicker/
+-rw-rw-rw-   0        0        0     4195 2023-06-24 04:10:02.000000 ARIclicker-0.3.4/ARIclicker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 04:11:06.754696 ARIclicker-0.3.4/ARIclicker.egg-info/
+-rw-rw-rw-   0        0        0     1792 2023-06-24 04:11:06.000000 ARIclicker-0.3.4/ARIclicker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-06-24 04:11:06.000000 ARIclicker-0.3.4/ARIclicker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 04:11:06.000000 ARIclicker-0.3.4/ARIclicker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-24 04:11:06.000000 ARIclicker-0.3.4/ARIclicker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 04:11:06.000000 ARIclicker-0.3.4/ARIclicker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1792 2023-06-24 04:11:06.754696 ARIclicker-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1436 2023-06-24 04:09:50.000000 ARIclicker-0.3.4/README.md
+-rw-rw-rw-   0        0        0     1093 2023-06-22 03:55:50.000000 ARIclicker-0.3.4/license.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 04:11:06.754696 ARIclicker-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      696 2023-06-24 04:10:35.000000 ARIclicker-0.3.4/setup.py
```

### Comparing `ARIclicker-0.2.3/ARIclicker/__init__.py` & `ARIclicker-0.3.4/ARIclicker/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,19 +30,25 @@
         mouse=Controller()
         while self.program_running:
             while self.running:
                 mouse.click(self.button)
                 time.sleep(random.uniform(self.delay_min, self.delay_max))
 
 
-def autoclick(start_stop_key_character, end_key_character, delay_min, delay_max, button):
+def autoclick(start_stop_key_character, end_key_character, button,delay_min=None, delay_max=None, delay=None ):
     if button == "left":
         button = Button.left
     if button == "right":
         button = Button.right
+    if delay_min!=None:
+        if delay_max==None or delay!=None:
+            raise Exception
+    else:
+        if delay_min!=None or delay==None:
+            raise Exception
     start_stop_key = KeyCode(char=start_stop_key_character)
     stop_key = KeyCode(char=end_key_character)
     mouse = pynput.mouse.Controller()
     click_thread = ClickMouse(delay_min, delay_max, button)
     click_thread.start()
 
     def on_press(key):
@@ -98,16 +104,21 @@
                 press_thread.start_pressing()
         elif key == stop_key:
             press_thread.exit()
             listener.stop()
     with Listener(on_press=on_press) as listener:
         listener.join()
 
-def quickclick(key_start,key_stop,program_stop_key=None):
-  
+def quickclick(key_start,key_stop,program_stop_key=None,delay_min=None,delay_max=None,delay=None):
+    if delay_min!=None:
+        if delay_max==None or delay!=None:
+            raise Exception
+    else:
+        if delay_min!=None or delay==None:
+            raise Exception  
     def func(key_start,key_stop):
        while True:
             keyboard.wait(key_start)
             time.sleep(0.1)
             while True:
                 pyautogui.click()
                 if keyboard.is_pressed(key_stop):
@@ -116,11 +127,8 @@
     def detect(key):
         while True:
             if keyboard.is_pressed(key):
                 exit(0)       
     t1=threading.Thread(target=func,args=(key_start,key_stop)).start()
     if program_stop_key!=None:
         t2 =threading.Thread(target=detect,args=(program_stop_key)).start()
-        
-    
-    
-
+
```

### Comparing `ARIclicker-0.2.3/ARIclicker.egg-info/PKG-INFO` & `ARIclicker-0.3.4/ARIclicker.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARIclicker
-Version: 0.2.3
+Version: 0.3.4
 Summary: AutoRandomIntervalClicker
 Home-page: UNKNOWN
 Author: lin_zhe
 Author-email: 2081812728@qq.com
 Maintainer: lin_zhe
 License: MIT License
 Keywords: AutoRandomIntervalClicker
@@ -25,41 +25,54 @@
 
 You need to install **ARIclicker**: Open `cmd` and type `pip install ARIclicker`
 
 ### Function:
 
 **syntax:**
 
-clicker:
+**clicker**:
+
+(autoclick)
 `
 ARIclicker.autoclick("start_pause_key","end_key","min_interval(sec)","max_interval(sec)","button")
 `
 
-presser:
+(quickclick)
+`
+ARIclicker.quickclick(key_start,key_stop,program_stop_key=None)
+`
+
+**presser**:
 `
 ARIclicker.autopress("start_pause_key","end_key","pressed_button")
 `
 
 example 1:
 <pre>
 	import ARIclicker 
 	ARIclicker.autoclick("a","b","0.1","1","left")
-	
 </pre>
 
 **explanation:** If you press the "a" key, clicking will start. When you press the "a" key again, clicking will pause. When you press the "b" key, the program will exit. The range of click intervals is between 0.1 and 1 second, and the left mouse button is the key clicked.
 
 example 2:
 <pre>
 	import ARIclicker
 	ARIclicker.autopress("a","b","c")
 </pre>
 
+
 **explanation:** If you press the "a" key,pressing will start.When you press the "a" key again, pressing will pause.When you press the "b" key, the program will exit.The 'c' key represents the key that will be pressed.
 
+example 3:
+<pre>
+	import ARIclicker
+	ARIclicker.quickclick("a","b")
+</pre>
+
 
  ### **have fun~**
```

### Comparing `ARIclicker-0.2.3/PKG-INFO` & `ARIclicker-0.3.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARIclicker
-Version: 0.2.3
+Version: 0.3.4
 Summary: AutoRandomIntervalClicker
 Home-page: UNKNOWN
 Author: lin_zhe
 Author-email: 2081812728@qq.com
 Maintainer: lin_zhe
 License: MIT License
 Keywords: AutoRandomIntervalClicker
@@ -25,41 +25,54 @@
 
 You need to install **ARIclicker**: Open `cmd` and type `pip install ARIclicker`
 
 ### Function:
 
 **syntax:**
 
-clicker:
+**clicker**:
+
+(autoclick)
 `
 ARIclicker.autoclick("start_pause_key","end_key","min_interval(sec)","max_interval(sec)","button")
 `
 
-presser:
+(quickclick)
+`
+ARIclicker.quickclick(key_start,key_stop,program_stop_key=None)
+`
+
+**presser**:
 `
 ARIclicker.autopress("start_pause_key","end_key","pressed_button")
 `
 
 example 1:
 <pre>
 	import ARIclicker 
 	ARIclicker.autoclick("a","b","0.1","1","left")
-	
 </pre>
 
 **explanation:** If you press the "a" key, clicking will start. When you press the "a" key again, clicking will pause. When you press the "b" key, the program will exit. The range of click intervals is between 0.1 and 1 second, and the left mouse button is the key clicked.
 
 example 2:
 <pre>
 	import ARIclicker
 	ARIclicker.autopress("a","b","c")
 </pre>
 
+
 **explanation:** If you press the "a" key,pressing will start.When you press the "a" key again, pressing will pause.When you press the "b" key, the program will exit.The 'c' key represents the key that will be pressed.
 
+example 3:
+<pre>
+	import ARIclicker
+	ARIclicker.quickclick("a","b")
+</pre>
+
 
  ### **have fun~**
```

### Comparing `ARIclicker-0.2.3/README.md` & `ARIclicker-0.3.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,41 +10,54 @@
 
 You need to install **ARIclicker**: Open `cmd` and type `pip install ARIclicker`
 
 ### Function:
 
 **syntax:**
 
-clicker:
+**clicker**:
+
+(autoclick)
 `
 ARIclicker.autoclick("start_pause_key","end_key","min_interval(sec)","max_interval(sec)","button")
 `
 
-presser:
+(quickclick)
+`
+ARIclicker.quickclick(key_start,key_stop,program_stop_key=None)
+`
+
+**presser**:
 `
 ARIclicker.autopress("start_pause_key","end_key","pressed_button")
 `
 
 example 1:
 <pre>
 	import ARIclicker 
 	ARIclicker.autoclick("a","b","0.1","1","left")
-	
 </pre>
 
 **explanation:** If you press the "a" key, clicking will start. When you press the "a" key again, clicking will pause. When you press the "b" key, the program will exit. The range of click intervals is between 0.1 and 1 second, and the left mouse button is the key clicked.
 
 example 2:
 <pre>
 	import ARIclicker
 	ARIclicker.autopress("a","b","c")
 </pre>
 
+
 **explanation:** If you press the "a" key,pressing will start.When you press the "a" key again, pressing will pause.When you press the "b" key, the program will exit.The 'c' key represents the key that will be pressed.
 
+example 3:
+<pre>
+	import ARIclicker
+	ARIclicker.quickclick("a","b")
+</pre>
+
 
  ### **have fun~**
```

### Comparing `ARIclicker-0.2.3/license.txt` & `ARIclicker-0.3.4/license.txt`

 * *Files identical despite different names*

### Comparing `ARIclicker-0.2.3/setup.py` & `ARIclicker-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setup(
     name = 'ARIclicker',
-    version = '0.2.3',
+    version = '0.3.4',
     maintainer='lin_zhe',
     keywords='AutoRandomIntervalClicker',
     description = 'AutoRandomIntervalClicker',
     long_description_content_type='text/markdown',
     long_description=long_description,
     license = 'MIT License',
     author = 'lin_zhe',
```

