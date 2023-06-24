# Comparing `tmp/tkcomponents-2.1.1.tar.gz` & `tmp/tkcomponents-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tkcomponents-2.1.1.tar", last modified: Mon Sep  5 15:24:47 2022, max compression
+gzip compressed data, was "tkcomponents-2.1.2.tar", last modified: Sat Jun 24 05:09:47 2023, max compression
```

## Comparing `tkcomponents-2.1.1.tar` & `tkcomponents-2.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2022-09-05 15:24:47.645131 tkcomponents-2.1.1/
--rw-rw-rw-   0        0        0     1087 2021-02-07 14:49:35.000000 tkcomponents-2.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       40 2021-02-07 14:36:16.000000 tkcomponents-2.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2443 2022-09-05 15:24:47.645131 tkcomponents-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2022-02-25 13:47:36.000000 tkcomponents-2.1.1/README.md
--rw-rw-rw-   0        0        0       42 2022-09-05 15:24:47.645131 tkcomponents-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1228 2022-09-05 15:23:36.000000 tkcomponents-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-05 15:24:47.600250 tkcomponents-2.1.1/tkcomponents/
--rw-rw-rw-   0        0        0       34 2020-11-29 03:48:50.000000 tkcomponents-2.1.1/tkcomponents/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-05 15:24:47.620198 tkcomponents-2.1.1/tkcomponents/abstractcomponents/
--rw-rw-rw-   0        0        0       90 2021-02-08 14:22:06.000000 tkcomponents-2.1.1/tkcomponents/abstractcomponents/__init__.py
--rw-rw-rw-   0        0        0     2180 2022-02-25 14:01:02.000000 tkcomponents-2.1.1/tkcomponents/abstractcomponents/timedframe.py
--rw-rw-rw-   0        0        0     3018 2022-02-25 14:01:02.000000 tkcomponents-2.1.1/tkcomponents/abstractcomponents/verticalscrollframe.py
-drwxrwxrwx   0        0        0        0 2022-09-05 15:24:47.631168 tkcomponents-2.1.1/tkcomponents/basiccomponents/
--rw-rw-rw-   0        0        0      472 2021-10-01 23:21:42.000000 tkcomponents-2.1.1/tkcomponents/basiccomponents/__init__.py
--rw-rw-rw-   0        0        0     1612 2022-02-25 14:01:02.000000 tkcomponents-2.1.1/tkcomponents/basiccomponents/alert.py
--rw-rw-rw-   0        0        0     2322 2021-11-02 01:05:45.000000 tkcomponents-2.1.1/tkcomponents/basiccomponents/buttonlistbox.py
-drwxrwxrwx   0        0        0        0 2022-09-05 15:24:47.642139 tkcomponents-2.1.1/tkcomponents/basiccomponents/classes/
--rw-rw-rw-   0        0        0      338 2020-11-18 00:08:16.000000 tkcomponents-2.1.1/tkcomponents/basiccomponents/classes/dateticker.py
--rw-rw-rw-   0        0        0     1175 2021-02-09 06:25:11.000000 tkcomponents-2.1.1/tkcomponents/basiccomponents/classes/timer.py
--rw-rw-rw-   0        0        0      203 2020-12-25 08:29:15.000000 tkcomponents-2.1.1/tkcomponents/basiccomponents/constants.py
--rw-rw-rw-   0        0        0     3068 2022-02-25 14:01:02.000000 tkcomponents-2.1.1/tkcomponents/basiccomponents/datestepper.py
--rw-rw-rw-   0        0        0      850 2022-02-25 14:01:02.000000 tkcomponents-2.1.1/tkcomponents/basiccomponents/labelwrapper.py
--rw-rw-rw-   0        0        0     4981 2022-02-25 14:01:02.000000 tkcomponents-2.1.1/tkcomponents/basiccomponents/numberstepper.py
--rw-rw-rw-   0        0        0     2568 2022-02-25 14:01:02.000000 tkcomponents-2.1.1/tkcomponents/basiccomponents/numbersteppertable.py
--rw-rw-rw-   0        0        0     3577 2022-02-25 14:01:02.000000 tkcomponents-2.1.1/tkcomponents/basiccomponents/progressbar.py
--rw-rw-rw-   0        0        0     2861 2022-02-25 14:01:02.000000 tkcomponents-2.1.1/tkcomponents/basiccomponents/stringeditor.py
--rw-rw-rw-   0        0        0     3259 2022-02-25 14:01:02.000000 tkcomponents-2.1.1/tkcomponents/basiccomponents/textcarousel.py
--rw-rw-rw-   0        0        0     2743 2022-02-25 14:01:02.000000 tkcomponents-2.1.1/tkcomponents/basiccomponents/timercontrol.py
--rw-rw-rw-   0        0        0     1575 2022-02-25 14:01:02.000000 tkcomponents-2.1.1/tkcomponents/basiccomponents/togglebutton.py
--rw-rw-rw-   0        0        0     7621 2022-02-25 14:08:12.000000 tkcomponents-2.1.1/tkcomponents/component.py
-drwxrwxrwx   0        0        0        0 2022-09-05 15:24:47.644133 tkcomponents-2.1.1/tkcomponents/extensions/
--rw-rw-rw-   0        0        0       36 2021-02-08 12:20:34.000000 tkcomponents-2.1.1/tkcomponents/extensions/__init__.py
--rw-rw-rw-   0        0        0     1590 2022-07-20 00:30:12.000000 tkcomponents-2.1.1/tkcomponents/extensions/gridhelper.py
-drwxrwxrwx   0        0        0        0 2022-09-05 15:24:47.617205 tkcomponents-2.1.1/tkcomponents.egg-info/
--rw-rw-rw-   0        0        0     2443 2022-09-05 15:24:47.000000 tkcomponents-2.1.1/tkcomponents.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1165 2022-09-05 15:24:47.000000 tkcomponents-2.1.1/tkcomponents.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-05 15:24:47.000000 tkcomponents-2.1.1/tkcomponents.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2022-09-05 15:24:47.000000 tkcomponents-2.1.1/tkcomponents.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-09-05 15:24:47.000000 tkcomponents-2.1.1/tkcomponents.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 05:09:47.371451 tkcomponents-2.1.2/
+-rw-rw-rw-   0        0        0     1087 2021-02-07 14:49:35.000000 tkcomponents-2.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       40 2021-02-07 14:36:16.000000 tkcomponents-2.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2023 2023-06-24 05:09:47.371451 tkcomponents-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2022-02-25 13:47:36.000000 tkcomponents-2.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 05:09:47.371451 tkcomponents-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2023-06-24 05:09:13.000000 tkcomponents-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:09:47.320440 tkcomponents-2.1.2/tkcomponents/
+-rw-rw-rw-   0        0        0       34 2020-11-29 03:48:50.000000 tkcomponents-2.1.2/tkcomponents/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:09:47.345421 tkcomponents-2.1.2/tkcomponents/abstractcomponents/
+-rw-rw-rw-   0        0        0       90 2021-02-08 14:22:06.000000 tkcomponents-2.1.2/tkcomponents/abstractcomponents/__init__.py
+-rw-rw-rw-   0        0        0     2180 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/abstractcomponents/timedframe.py
+-rw-rw-rw-   0        0        0     3018 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/abstractcomponents/verticalscrollframe.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:09:47.356421 tkcomponents-2.1.2/tkcomponents/basiccomponents/
+-rw-rw-rw-   0        0        0      472 2021-10-01 23:21:42.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/__init__.py
+-rw-rw-rw-   0        0        0     1612 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/alert.py
+-rw-rw-rw-   0        0        0     2322 2021-11-02 01:05:45.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/buttonlistbox.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:09:47.368451 tkcomponents-2.1.2/tkcomponents/basiccomponents/classes/
+-rw-rw-rw-   0        0        0      338 2020-11-18 00:08:16.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/classes/dateticker.py
+-rw-rw-rw-   0        0        0     1175 2021-02-09 06:25:11.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/classes/timer.py
+-rw-rw-rw-   0        0        0      203 2020-12-25 08:29:15.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/constants.py
+-rw-rw-rw-   0        0        0     3068 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/datestepper.py
+-rw-rw-rw-   0        0        0      850 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/labelwrapper.py
+-rw-rw-rw-   0        0        0     4981 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/numberstepper.py
+-rw-rw-rw-   0        0        0     2568 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/numbersteppertable.py
+-rw-rw-rw-   0        0        0     3577 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/progressbar.py
+-rw-rw-rw-   0        0        0     2861 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/stringeditor.py
+-rw-rw-rw-   0        0        0     3259 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/textcarousel.py
+-rw-rw-rw-   0        0        0     2743 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/timercontrol.py
+-rw-rw-rw-   0        0        0     1575 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/togglebutton.py
+-rw-rw-rw-   0        0        0     7621 2022-02-25 14:08:12.000000 tkcomponents-2.1.2/tkcomponents/component.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:09:47.370421 tkcomponents-2.1.2/tkcomponents/extensions/
+-rw-rw-rw-   0        0        0       36 2021-02-08 12:20:34.000000 tkcomponents-2.1.2/tkcomponents/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1590 2022-07-20 00:30:12.000000 tkcomponents-2.1.2/tkcomponents/extensions/gridhelper.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:09:47.342451 tkcomponents-2.1.2/tkcomponents.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-06-24 05:09:47.000000 tkcomponents-2.1.2/tkcomponents.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1165 2023-06-24 05:09:47.000000 tkcomponents-2.1.2/tkcomponents.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 05:09:47.000000 tkcomponents-2.1.2/tkcomponents.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-24 05:09:47.000000 tkcomponents-2.1.2/tkcomponents.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-24 05:09:47.000000 tkcomponents-2.1.2/tkcomponents.egg-info/top_level.txt
```

### Comparing `tkcomponents-2.1.1/LICENSE.txt` & `tkcomponents-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/PKG-INFO` & `tkcomponents-2.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 Metadata-Version: 2.1
 Name: tkcomponents
-Version: 2.1.1
+Version: 2.1.2
 Summary: An OOP framework for Tkinter, inspired by React
 Home-page: https://github.com/immijimmi/tkcomponents
+Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v2.1.2.tar.gz
 Author: immijimmi
-Author-email: imranhamid99@msn.com
+Author-email: immijimmi1@gmail.com
 License: MIT
-Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v2.1.1.tar.gz
-Description: # tkcomponents
-        
-        ###### An OOP framework for Tkinter, inspired by React
-        
-        ## Quickstart
-        
-        ### Setup
-        
-        Below is an example of a custom component, a number label which updates its value periodically.
-        
-        ```python
-        from tkinter import Label, IntVar
-        
-        from tkcomponents import Component
-        
-        
-        class Counter(Component):
-            def __init__(self, container):
-                super().__init__(container, update_interval_ms=250)  # The component will update 4 times per second
-        
-                self._count__var = IntVar()
-                self._count__var.set(0)
-        
-            @property
-            def _needs_render(self):
-                return self._count__var.get() % 5 == 0  # A full re-render will trigger on multiples of 5
-        
-            def _update(self):
-                current_count = self._count__var.get()
-        
-                self._count__var.set(current_count+1)  # The counter will increase by 1 each update, a total of +4 per second
-        
-            def _render(self):
-                Label(self._frame, textvariable=self._count__var).pack()
-        ```
-        
-        ### App Boilerplate
-        ```python
-        from tkinter import Tk
-        
-        
-        class App:
-            def __init__(self):
-                self.window = Tk()
-        
-                Counter(self.window).render().pack()  # Note that .render() is called from outside the component, not ._render()
-        
-                self.window.mainloop()
-        
-        if __name__ == "__main__":
-            App()
-        ```
-        
 Keywords: ui,gui,graphical,user,interface
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# tkcomponents
+
+###### An OOP framework for Tkinter, inspired by React
+
+## Quickstart
+
+### Setup
+
+Below is an example of a custom component, a number label which updates its value periodically.
+
+```python
+from tkinter import Label, IntVar
+
+from tkcomponents import Component
+
+
+class Counter(Component):
+    def __init__(self, container):
+        super().__init__(container, update_interval_ms=250)  # The component will update 4 times per second
+
+        self._count__var = IntVar()
+        self._count__var.set(0)
+
+    @property
+    def _needs_render(self):
+        return self._count__var.get() % 5 == 0  # A full re-render will trigger on multiples of 5
+
+    def _update(self):
+        current_count = self._count__var.get()
+
+        self._count__var.set(current_count+1)  # The counter will increase by 1 each update, a total of +4 per second
+
+    def _render(self):
+        Label(self._frame, textvariable=self._count__var).pack()
+```
+
+### App Boilerplate
+```python
+from tkinter import Tk
+
+
+class App:
+    def __init__(self):
+        self.window = Tk()
+
+        Counter(self.window).render().pack()  # Note that .render() is called from outside the component, not ._render()
+
+        self.window.mainloop()
+
+if __name__ == "__main__":
+    App()
+```
```

### Comparing `tkcomponents-2.1.1/README.md` & `tkcomponents-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/setup.py` & `tkcomponents-2.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 
 setup(
     name="tkcomponents",
     packages=[
         "tkcomponents", "tkcomponents.extensions", "tkcomponents.basiccomponents", "tkcomponents.abstractcomponents",
         "tkcomponents.basiccomponents.classes"
     ],
-    version="2.1.1",
+    version="2.1.2",
     license="MIT",
     description="An OOP framework for Tkinter, inspired by React",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="immijimmi",
-    author_email="imranhamid99@msn.com",
+    author_email="immijimmi1@gmail.com",
     url="https://github.com/immijimmi/tkcomponents",
-    download_url="https://github.com/immijimmi/tkcomponents/archive/refs/tags/v2.1.1.tar.gz",
+    download_url="https://github.com/immijimmi/tkcomponents/archive/refs/tags/v2.1.2.tar.gz",
     keywords=[
         'ui', 'gui', 'graphical', 'user', 'interface'
     ],
     install_requires=[
-        'objectextensions~=2.0.0'
+        'objectextensions~=2.0.2'
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `tkcomponents-2.1.1/tkcomponents/abstractcomponents/timedframe.py` & `tkcomponents-2.1.2/tkcomponents/abstractcomponents/timedframe.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/tkcomponents/abstractcomponents/verticalscrollframe.py` & `tkcomponents-2.1.2/tkcomponents/abstractcomponents/verticalscrollframe.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/tkcomponents/basiccomponents/alert.py` & `tkcomponents-2.1.2/tkcomponents/basiccomponents/alert.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/tkcomponents/basiccomponents/buttonlistbox.py` & `tkcomponents-2.1.2/tkcomponents/basiccomponents/buttonlistbox.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/tkcomponents/basiccomponents/classes/timer.py` & `tkcomponents-2.1.2/tkcomponents/basiccomponents/classes/timer.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/tkcomponents/basiccomponents/datestepper.py` & `tkcomponents-2.1.2/tkcomponents/basiccomponents/datestepper.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/tkcomponents/basiccomponents/labelwrapper.py` & `tkcomponents-2.1.2/tkcomponents/basiccomponents/labelwrapper.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/tkcomponents/basiccomponents/numberstepper.py` & `tkcomponents-2.1.2/tkcomponents/basiccomponents/numberstepper.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/tkcomponents/basiccomponents/numbersteppertable.py` & `tkcomponents-2.1.2/tkcomponents/basiccomponents/numbersteppertable.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/tkcomponents/basiccomponents/progressbar.py` & `tkcomponents-2.1.2/tkcomponents/basiccomponents/progressbar.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/tkcomponents/basiccomponents/stringeditor.py` & `tkcomponents-2.1.2/tkcomponents/basiccomponents/stringeditor.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/tkcomponents/basiccomponents/textcarousel.py` & `tkcomponents-2.1.2/tkcomponents/basiccomponents/textcarousel.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/tkcomponents/basiccomponents/timercontrol.py` & `tkcomponents-2.1.2/tkcomponents/basiccomponents/timercontrol.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/tkcomponents/basiccomponents/togglebutton.py` & `tkcomponents-2.1.2/tkcomponents/basiccomponents/togglebutton.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/tkcomponents/component.py` & `tkcomponents-2.1.2/tkcomponents/component.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/tkcomponents/extensions/gridhelper.py` & `tkcomponents-2.1.2/tkcomponents/extensions/gridhelper.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.1/tkcomponents.egg-info/PKG-INFO` & `tkcomponents-2.1.2/tkcomponents.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 Metadata-Version: 2.1
 Name: tkcomponents
-Version: 2.1.1
+Version: 2.1.2
 Summary: An OOP framework for Tkinter, inspired by React
 Home-page: https://github.com/immijimmi/tkcomponents
+Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v2.1.2.tar.gz
 Author: immijimmi
-Author-email: imranhamid99@msn.com
+Author-email: immijimmi1@gmail.com
 License: MIT
-Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v2.1.1.tar.gz
-Description: # tkcomponents
-        
-        ###### An OOP framework for Tkinter, inspired by React
-        
-        ## Quickstart
-        
-        ### Setup
-        
-        Below is an example of a custom component, a number label which updates its value periodically.
-        
-        ```python
-        from tkinter import Label, IntVar
-        
-        from tkcomponents import Component
-        
-        
-        class Counter(Component):
-            def __init__(self, container):
-                super().__init__(container, update_interval_ms=250)  # The component will update 4 times per second
-        
-                self._count__var = IntVar()
-                self._count__var.set(0)
-        
-            @property
-            def _needs_render(self):
-                return self._count__var.get() % 5 == 0  # A full re-render will trigger on multiples of 5
-        
-            def _update(self):
-                current_count = self._count__var.get()
-        
-                self._count__var.set(current_count+1)  # The counter will increase by 1 each update, a total of +4 per second
-        
-            def _render(self):
-                Label(self._frame, textvariable=self._count__var).pack()
-        ```
-        
-        ### App Boilerplate
-        ```python
-        from tkinter import Tk
-        
-        
-        class App:
-            def __init__(self):
-                self.window = Tk()
-        
-                Counter(self.window).render().pack()  # Note that .render() is called from outside the component, not ._render()
-        
-                self.window.mainloop()
-        
-        if __name__ == "__main__":
-            App()
-        ```
-        
 Keywords: ui,gui,graphical,user,interface
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# tkcomponents
+
+###### An OOP framework for Tkinter, inspired by React
+
+## Quickstart
+
+### Setup
+
+Below is an example of a custom component, a number label which updates its value periodically.
+
+```python
+from tkinter import Label, IntVar
+
+from tkcomponents import Component
+
+
+class Counter(Component):
+    def __init__(self, container):
+        super().__init__(container, update_interval_ms=250)  # The component will update 4 times per second
+
+        self._count__var = IntVar()
+        self._count__var.set(0)
+
+    @property
+    def _needs_render(self):
+        return self._count__var.get() % 5 == 0  # A full re-render will trigger on multiples of 5
+
+    def _update(self):
+        current_count = self._count__var.get()
+
+        self._count__var.set(current_count+1)  # The counter will increase by 1 each update, a total of +4 per second
+
+    def _render(self):
+        Label(self._frame, textvariable=self._count__var).pack()
+```
+
+### App Boilerplate
+```python
+from tkinter import Tk
+
+
+class App:
+    def __init__(self):
+        self.window = Tk()
+
+        Counter(self.window).render().pack()  # Note that .render() is called from outside the component, not ._render()
+
+        self.window.mainloop()
+
+if __name__ == "__main__":
+    App()
+```
```

### Comparing `tkcomponents-2.1.1/tkcomponents.egg-info/SOURCES.txt` & `tkcomponents-2.1.2/tkcomponents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

