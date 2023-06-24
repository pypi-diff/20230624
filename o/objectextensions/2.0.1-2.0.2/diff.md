# Comparing `tmp/objectextensions-2.0.1.tar.gz` & `tmp/objectextensions-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\objectextensions-2.0.1.tar", last modified: Fri Oct  7 15:56:52 2022, max compression
+gzip compressed data, was "objectextensions-2.0.2.tar", last modified: Sat Jun 24 03:58:51 2023, max compression
```

## Comparing `objectextensions-2.0.1.tar` & `objectextensions-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-10-07 15:56:52.386310 objectextensions-2.0.1/
--rw-rw-rw-   0        0        0     1087 2021-01-16 15:06:27.000000 objectextensions-2.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       40 2021-01-15 22:18:51.000000 objectextensions-2.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    10630 2022-10-07 15:56:52.386310 objectextensions-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8414 2022-09-05 10:54:48.000000 objectextensions-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-10-07 15:56:52.372348 objectextensions-2.0.1/objectextensions/
--rw-rw-rw-   0        0        0      127 2022-09-05 09:42:36.000000 objectextensions-2.0.1/objectextensions/__init__.py
--rw-rw-rw-   0        0        0     1804 2022-09-05 10:37:57.000000 objectextensions-2.0.1/objectextensions/extendable.py
--rw-rw-rw-   0        0        0     4409 2022-09-04 11:49:53.000000 objectextensions-2.0.1/objectextensions/extension.py
--rw-rw-rw-   0        0        0     1397 2022-09-16 15:12:54.000000 objectextensions-2.0.1/objectextensions/methods.py
-drwxrwxrwx   0        0        0        0 2022-10-07 15:56:52.385313 objectextensions-2.0.1/objectextensions.egg-info/
--rw-rw-rw-   0        0        0    10630 2022-10-07 15:56:52.000000 objectextensions-2.0.1/objectextensions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2022-10-07 15:56:52.000000 objectextensions-2.0.1/objectextensions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-07 15:56:52.000000 objectextensions-2.0.1/objectextensions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2022-10-07 15:56:52.000000 objectextensions-2.0.1/objectextensions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2022-10-07 15:56:52.000000 objectextensions-2.0.1/objectextensions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-07 15:56:52.387308 objectextensions-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1061 2022-10-07 15:54:08.000000 objectextensions-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 03:58:51.516879 objectextensions-2.0.2/
+-rw-rw-rw-   0        0        0     1087 2021-01-16 15:06:27.000000 objectextensions-2.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       40 2021-01-15 22:18:51.000000 objectextensions-2.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     9138 2023-06-24 03:58:51.516879 objectextensions-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8414 2022-09-05 10:54:48.000000 objectextensions-2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 03:58:51.498906 objectextensions-2.0.2/objectextensions/
+-rw-rw-rw-   0        0        0      127 2022-09-05 09:42:36.000000 objectextensions-2.0.2/objectextensions/__init__.py
+-rw-rw-rw-   0        0        0     1804 2022-09-05 10:37:57.000000 objectextensions-2.0.2/objectextensions/extendable.py
+-rw-rw-rw-   0        0        0     4409 2022-09-04 11:49:53.000000 objectextensions-2.0.2/objectextensions/extension.py
+-rw-rw-rw-   0        0        0     1397 2022-09-16 15:12:54.000000 objectextensions-2.0.2/objectextensions/methods.py
+drwxrwxrwx   0        0        0        0 2023-06-24 03:58:51.515908 objectextensions-2.0.2/objectextensions.egg-info/
+-rw-rw-rw-   0        0        0     9138 2023-06-24 03:58:51.000000 objectextensions-2.0.2/objectextensions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-06-24 03:58:51.000000 objectextensions-2.0.2/objectextensions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 03:58:51.000000 objectextensions-2.0.2/objectextensions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-24 03:58:51.000000 objectextensions-2.0.2/objectextensions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-24 03:58:51.000000 objectextensions-2.0.2/objectextensions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 03:58:51.516879 objectextensions-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1062 2023-06-24 03:56:09.000000 objectextensions-2.0.2/setup.py
```

### Comparing `objectextensions-2.0.1/LICENSE.txt` & `objectextensions-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `objectextensions-2.0.1/PKG-INFO` & `objectextensions-2.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,204 +1,186 @@
-Metadata-Version: 2.1
-Name: objectextensions
-Version: 2.0.1
-Summary: A basic framework for implementing an extension pattern
-Home-page: https://github.com/immijimmi/objectextensions
-Author: immijimmi
-Author-email: immijimmi1@gmail.com
-License: MIT
-Download-URL: https://github.com/immijimmi/objectextensions/archive/refs/tags/v2.0.1.tar.gz
-Description: # Object Extensions
-        
-        ###### A basic framework for implementing an extension pattern
-        
-        ## Summary
-        
-        The point of this framework is to provide a more modular alternative to object inheritance.
-        
-        **Consider the following use case:** You have an abstract class `Car` intended to represent a car, and need a pattern that allows you to *optionally* add more features.
-        For example, you may want to add a convertible roof or a touchscreen on the dashboard, but these features will not necessarily be added to every subclass of `Car` you create.
-        
-        Applying standard OOP here means you would need to make a subclass every time a new combination of these optional features is needed.
-        In the above case, you may need one subclass for a car with a convertible roof, one subclass for a car with a touchscreen, and one that has both features. As the amount of optional features increases,
-        the amount of possible combinations skyrockets. This is not a scalable solution to the problem.
-        
-        Object Extensions is an elegant way to handle scenarios such as this one. Rather than creating a new subclass for each possible combination,
-        you create one extension representing each feature. When you need to create a car with a particular set of features,
-        you take the parent class and pass it the exact set of extensions you want to apply via the `.with_extensions()` method as the need arises.
-        
-        Note that this pattern is intended to be used alongside inheritance, not to replace it entirely. The two can be mixed without issue, such that
-        (for example) a subclass could extend a parent class that has pre-applied extensions like so:
-        ```python
-        class SpecificCarModel(Car.with_extensions(TouchscreenDash)):
-            pass
-        ```
-        
-        ## Quickstart
-        
-        ### Setup
-        
-        Below is an example of an extendable class, and an example extension that can be applied to it.
-        
-        ```python
-        from objectextensions import Extendable
-        
-        
-        class HashList(Extendable):
-            """
-            A basic example class with some data and methods.
-            Inheriting Extendable allows this class to be modified with extensions
-            """
-        
-            def __init__(self, iterable=()):
-                super().__init__()
-        
-                self.values = {}
-                self.list = []
-        
-                for value in iterable:
-                    self.append(value)
-        
-            def append(self, item):
-                self.list.append(item)
-                self.values[item] = self.values.get(item, []) + [len(self.list) - 1]
-        
-            def index(self, item):
-                """
-                Returns all indexes containing the specified item.
-                Much lower time complexity than in a typical list due to dict lookup usage
-                """
-        
-                if item not in self.values:
-                    raise ValueError(f"{item} is not in hashlist")
-        
-                return self.values[item]
-        ```
-        ```python
-        from objectextensions import Extension
-        
-        
-        class Listener(Extension):
-            """
-            This extension class is written to apply a counter to the HashList class,
-            which increments any time .append() is called
-            """
-        
-            @staticmethod
-            def can_extend(target_cls):
-                return issubclass(target_cls, HashList)
-        
-            @staticmethod
-            def extend(target_cls):
-                Extension._set(target_cls, "increment_append_count", Listener.__increment_append_count)
-        
-                Extension._wrap(target_cls, "__init__", Listener.__wrap_init)
-                Extension._wrap(target_cls, 'append', Listener.__wrap_append)
-        
-            def __wrap_init(self, *args, **kwargs):
-                Extension._set(self, "append_count", 0)
-                yield
-        
-            def __wrap_append(self, *args, **kwargs):
-                yield
-                self.increment_append_count()
-        
-            def __increment_append_count(self):
-                self.append_count += 1
-        ```
-        
-        ### Instantiation
-        ```python
-        HashListWithListeners = HashList.with_extensions(Listener)
-        my_hashlist = HashListWithListeners(iterable=[5,2,4])
-        ```
-        or, for shorthand:
-        ```python
-        my_hashlist = HashList.with_extensions(Listener)(iterable=[5,2,4])
-        ```
-        
-        ### Result
-        ```python
-        >>> my_hashlist.append_count  # Attribute that was added by the Listener extension
-        3
-        >>> my_hashlist.append(7)  # Listener has wrapped this method with logic which increments .append_count
-        >>> my_hashlist.append_count
-        4
-        ```
-        
-        ## Functionality
-        
-        ### Properties
-        
-        Extendable.**extensions**  
-        &nbsp;&nbsp;&nbsp;&nbsp;Returns a reference to a tuple containing any applied extensions.  
-        &nbsp;
-        
-        Extendable.**extension_data**  
-        &nbsp;&nbsp;&nbsp;&nbsp;Returns a snapshot of the instance's extension data.  
-        &nbsp;&nbsp;&nbsp;&nbsp;This is intended to hold metadata optionally provided by extensions for the sake of introspection,  
-        &nbsp;&nbsp;&nbsp;&nbsp;and for communication between extensions.  
-        &nbsp;
-        
-        ### Methods
-        
-        Extendable.**with_extensions**(*cls, \*extensions: Type[Extension]*)  
-        &nbsp;&nbsp;&nbsp;&nbsp;Returns a subclass with the provided extensions applied to it.  
-        &nbsp;
-        
-        Extension.**can_extend**(*target_cls: Type[Extendable]*)  
-        &nbsp;&nbsp;&nbsp;&nbsp;Abstract staticmethod which must be overridden.  
-        &nbsp;&nbsp;&nbsp;&nbsp;Should return a bool indicating whether this Extension can be applied to the target class.  
-        &nbsp;
-        
-        Extension.**extend**(*target_cls: Type[Extendable]*)  
-        &nbsp;&nbsp;&nbsp;&nbsp;Abstract staticmethod which must be overridden.  
-        &nbsp;&nbsp;&nbsp;&nbsp;Any modification of the target class should take place in this function.  
-        &nbsp;
-        
-        Extension.**\_wrap**(*target_cls: Type[Extendable], method_name: str,*  
-        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*gen_func: Callable[..., Generator[None, Any, None]]*)  
-        &nbsp;&nbsp;&nbsp;&nbsp;Used to wrap an existing method on the target class.  
-        &nbsp;&nbsp;&nbsp;&nbsp;Passes copies of the method parameters to the generator function provided.  
-        &nbsp;&nbsp;&nbsp;&nbsp;The generator function should yield once,  
-        &nbsp;&nbsp;&nbsp;&nbsp;with the yield statement receiving a copy of the result of executing the core method.  
-        &nbsp;
-        
-        Extension.**\_set**(*target: Union[Type[Extendable], Extendable], attribute_name: str, value: Any*)  
-        &nbsp;&nbsp;&nbsp;&nbsp;Used to safely add a new attribute to an extendable class.  
-        
-        *Note: It is possible but not recommended to modify an instance rather than a class using this method.*  
-        &nbsp;&nbsp;&nbsp;&nbsp;*Will raise an error if the attribute already exists (for example, if another extension has already added it)*  
-        &nbsp;&nbsp;&nbsp;&nbsp;*to ensure compatibility issues are flagged and can be dealt with easily.*  
-        &nbsp;
-        
-        Extension.**\_set_property**(*target: Union[Type[Extendable], Extendable], property_name: str, value: Callable[[Extendable], Any]*)  
-        &nbsp;&nbsp;&nbsp;&nbsp;Used to safely add a new property to an extendable class.  
-        
-        *Note: It is possible but not recommended to modify an instance rather than a class using this method.*  
-        &nbsp;&nbsp;&nbsp;&nbsp;*Will raise an error if the attribute already exists (for example, if another extension has already added it)*  
-        &nbsp;&nbsp;&nbsp;&nbsp;*to ensure compatibility issues are flagged and can be dealt with easily.*  
-        &nbsp;
-        
-        Extension.**\_set_setter**(*target: Union[Type[Extendable], Extendable], setter_name: str, linked_property_name: str,*  
-        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*value: Callable[[Extendable, Any], Any]*)  
-        &nbsp;&nbsp;&nbsp;&nbsp;Used to safely add a new setter to an extendable class.  
-        
-        *Note: It is possible but not recommended to modify an instance rather than a class using this method.*  
-        &nbsp;&nbsp;&nbsp;&nbsp;*If the property this setter is paired with does not use the same attribute name,*  
-        &nbsp;&nbsp;&nbsp;&nbsp;*and the setter's name already exists on the class (for example, if another extension has already added it),*  
-        &nbsp;&nbsp;&nbsp;&nbsp;*an error will be raised. This is to ensure compatibility issues are flagged and can be dealt with easily.*  
-        &nbsp;
-        
-        ## Additional Info
-        
-        - As extensions do not properly invoke name mangling, adding private members via extensions is discouraged; doing so may lead to unintended behaviour.
-        Using protected members instead is encouraged, as name mangling does not come into play in this case.
-        
-Keywords: extensions,plugins
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
+# Object Extensions
+
+###### A basic framework for implementing an extension pattern
+
+## Summary
+
+The point of this framework is to provide a more modular alternative to object inheritance.
+
+**Consider the following use case:** You have an abstract class `Car` intended to represent a car, and need a pattern that allows you to *optionally* add more features.
+For example, you may want to add a convertible roof or a touchscreen on the dashboard, but these features will not necessarily be added to every subclass of `Car` you create.
+
+Applying standard OOP here means you would need to make a subclass every time a new combination of these optional features is needed.
+In the above case, you may need one subclass for a car with a convertible roof, one subclass for a car with a touchscreen, and one that has both features. As the amount of optional features increases,
+the amount of possible combinations skyrockets. This is not a scalable solution to the problem.
+
+Object Extensions is an elegant way to handle scenarios such as this one. Rather than creating a new subclass for each possible combination,
+you create one extension representing each feature. When you need to create a car with a particular set of features,
+you take the parent class and pass it the exact set of extensions you want to apply via the `.with_extensions()` method as the need arises.
+
+Note that this pattern is intended to be used alongside inheritance, not to replace it entirely. The two can be mixed without issue, such that
+(for example) a subclass could extend a parent class that has pre-applied extensions like so:
+```python
+class SpecificCarModel(Car.with_extensions(TouchscreenDash)):
+    pass
+```
+
+## Quickstart
+
+### Setup
+
+Below is an example of an extendable class, and an example extension that can be applied to it.
+
+```python
+from objectextensions import Extendable
+
+
+class HashList(Extendable):
+    """
+    A basic example class with some data and methods.
+    Inheriting Extendable allows this class to be modified with extensions
+    """
+
+    def __init__(self, iterable=()):
+        super().__init__()
+
+        self.values = {}
+        self.list = []
+
+        for value in iterable:
+            self.append(value)
+
+    def append(self, item):
+        self.list.append(item)
+        self.values[item] = self.values.get(item, []) + [len(self.list) - 1]
+
+    def index(self, item):
+        """
+        Returns all indexes containing the specified item.
+        Much lower time complexity than in a typical list due to dict lookup usage
+        """
+
+        if item not in self.values:
+            raise ValueError(f"{item} is not in hashlist")
+
+        return self.values[item]
+```
+```python
+from objectextensions import Extension
+
+
+class Listener(Extension):
+    """
+    This extension class is written to apply a counter to the HashList class,
+    which increments any time .append() is called
+    """
+
+    @staticmethod
+    def can_extend(target_cls):
+        return issubclass(target_cls, HashList)
+
+    @staticmethod
+    def extend(target_cls):
+        Extension._set(target_cls, "increment_append_count", Listener.__increment_append_count)
+
+        Extension._wrap(target_cls, "__init__", Listener.__wrap_init)
+        Extension._wrap(target_cls, 'append', Listener.__wrap_append)
+
+    def __wrap_init(self, *args, **kwargs):
+        Extension._set(self, "append_count", 0)
+        yield
+
+    def __wrap_append(self, *args, **kwargs):
+        yield
+        self.increment_append_count()
+
+    def __increment_append_count(self):
+        self.append_count += 1
+```
+
+### Instantiation
+```python
+HashListWithListeners = HashList.with_extensions(Listener)
+my_hashlist = HashListWithListeners(iterable=[5,2,4])
+```
+or, for shorthand:
+```python
+my_hashlist = HashList.with_extensions(Listener)(iterable=[5,2,4])
+```
+
+### Result
+```python
+>>> my_hashlist.append_count  # Attribute that was added by the Listener extension
+3
+>>> my_hashlist.append(7)  # Listener has wrapped this method with logic which increments .append_count
+>>> my_hashlist.append_count
+4
+```
+
+## Functionality
+
+### Properties
+
+Extendable.**extensions**  
+&nbsp;&nbsp;&nbsp;&nbsp;Returns a reference to a tuple containing any applied extensions.  
+&nbsp;
+
+Extendable.**extension_data**  
+&nbsp;&nbsp;&nbsp;&nbsp;Returns a snapshot of the instance's extension data.  
+&nbsp;&nbsp;&nbsp;&nbsp;This is intended to hold metadata optionally provided by extensions for the sake of introspection,  
+&nbsp;&nbsp;&nbsp;&nbsp;and for communication between extensions.  
+&nbsp;
+
+### Methods
+
+Extendable.**with_extensions**(*cls, \*extensions: Type[Extension]*)  
+&nbsp;&nbsp;&nbsp;&nbsp;Returns a subclass with the provided extensions applied to it.  
+&nbsp;
+
+Extension.**can_extend**(*target_cls: Type[Extendable]*)  
+&nbsp;&nbsp;&nbsp;&nbsp;Abstract staticmethod which must be overridden.  
+&nbsp;&nbsp;&nbsp;&nbsp;Should return a bool indicating whether this Extension can be applied to the target class.  
+&nbsp;
+
+Extension.**extend**(*target_cls: Type[Extendable]*)  
+&nbsp;&nbsp;&nbsp;&nbsp;Abstract staticmethod which must be overridden.  
+&nbsp;&nbsp;&nbsp;&nbsp;Any modification of the target class should take place in this function.  
+&nbsp;
+
+Extension.**\_wrap**(*target_cls: Type[Extendable], method_name: str,*  
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*gen_func: Callable[..., Generator[None, Any, None]]*)  
+&nbsp;&nbsp;&nbsp;&nbsp;Used to wrap an existing method on the target class.  
+&nbsp;&nbsp;&nbsp;&nbsp;Passes copies of the method parameters to the generator function provided.  
+&nbsp;&nbsp;&nbsp;&nbsp;The generator function should yield once,  
+&nbsp;&nbsp;&nbsp;&nbsp;with the yield statement receiving a copy of the result of executing the core method.  
+&nbsp;
+
+Extension.**\_set**(*target: Union[Type[Extendable], Extendable], attribute_name: str, value: Any*)  
+&nbsp;&nbsp;&nbsp;&nbsp;Used to safely add a new attribute to an extendable class.  
+
+*Note: It is possible but not recommended to modify an instance rather than a class using this method.*  
+&nbsp;&nbsp;&nbsp;&nbsp;*Will raise an error if the attribute already exists (for example, if another extension has already added it)*  
+&nbsp;&nbsp;&nbsp;&nbsp;*to ensure compatibility issues are flagged and can be dealt with easily.*  
+&nbsp;
+
+Extension.**\_set_property**(*target: Union[Type[Extendable], Extendable], property_name: str, value: Callable[[Extendable], Any]*)  
+&nbsp;&nbsp;&nbsp;&nbsp;Used to safely add a new property to an extendable class.  
+
+*Note: It is possible but not recommended to modify an instance rather than a class using this method.*  
+&nbsp;&nbsp;&nbsp;&nbsp;*Will raise an error if the attribute already exists (for example, if another extension has already added it)*  
+&nbsp;&nbsp;&nbsp;&nbsp;*to ensure compatibility issues are flagged and can be dealt with easily.*  
+&nbsp;
+
+Extension.**\_set_setter**(*target: Union[Type[Extendable], Extendable], setter_name: str, linked_property_name: str,*  
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*value: Callable[[Extendable, Any], Any]*)  
+&nbsp;&nbsp;&nbsp;&nbsp;Used to safely add a new setter to an extendable class.  
+
+*Note: It is possible but not recommended to modify an instance rather than a class using this method.*  
+&nbsp;&nbsp;&nbsp;&nbsp;*If the property this setter is paired with does not use the same attribute name,*  
+&nbsp;&nbsp;&nbsp;&nbsp;*and the setter's name already exists on the class (for example, if another extension has already added it),*  
+&nbsp;&nbsp;&nbsp;&nbsp;*an error will be raised. This is to ensure compatibility issues are flagged and can be dealt with easily.*  
+&nbsp;
+
+## Additional Info
+
+- As extensions do not properly invoke name mangling, adding private members via extensions is discouraged; doing so may lead to unintended behaviour.
+Using protected members instead is encouraged, as name mangling does not come into play in this case.
```

### Comparing `objectextensions-2.0.1/README.md` & `objectextensions-2.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: objectextensions
+Version: 2.0.2
+Summary: A basic framework for implementing an extension pattern
+Home-page: https://github.com/immijimmi/objectextensions
+Download-URL: https://github.com/immijimmi/objectextensions/archive/refs/tags/v2.0.2.tar.gz
+Author: immijimmi
+Author-email: immijimmi1@gmail.com
+License: MIT
+Keywords: extensions,plugins
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Object Extensions
 
 ###### A basic framework for implementing an extension pattern
 
 ## Summary
 
 The point of this framework is to provide a more modular alternative to object inheritance.
```

### Comparing `objectextensions-2.0.1/objectextensions/extendable.py` & `objectextensions-2.0.2/objectextensions/extendable.py`

 * *Files identical despite different names*

### Comparing `objectextensions-2.0.1/objectextensions/extension.py` & `objectextensions-2.0.2/objectextensions/extension.py`

 * *Files identical despite different names*

### Comparing `objectextensions-2.0.1/objectextensions/methods.py` & `objectextensions-2.0.2/objectextensions/methods.py`

 * *Files identical despite different names*

### Comparing `objectextensions-2.0.1/objectextensions.egg-info/PKG-INFO` & `objectextensions-2.0.2/objectextensions.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,204 +1,204 @@
 Metadata-Version: 2.1
 Name: objectextensions
-Version: 2.0.1
+Version: 2.0.2
 Summary: A basic framework for implementing an extension pattern
 Home-page: https://github.com/immijimmi/objectextensions
+Download-URL: https://github.com/immijimmi/objectextensions/archive/refs/tags/v2.0.2.tar.gz
 Author: immijimmi
 Author-email: immijimmi1@gmail.com
 License: MIT
-Download-URL: https://github.com/immijimmi/objectextensions/archive/refs/tags/v2.0.1.tar.gz
-Description: # Object Extensions
-        
-        ###### A basic framework for implementing an extension pattern
-        
-        ## Summary
-        
-        The point of this framework is to provide a more modular alternative to object inheritance.
-        
-        **Consider the following use case:** You have an abstract class `Car` intended to represent a car, and need a pattern that allows you to *optionally* add more features.
-        For example, you may want to add a convertible roof or a touchscreen on the dashboard, but these features will not necessarily be added to every subclass of `Car` you create.
-        
-        Applying standard OOP here means you would need to make a subclass every time a new combination of these optional features is needed.
-        In the above case, you may need one subclass for a car with a convertible roof, one subclass for a car with a touchscreen, and one that has both features. As the amount of optional features increases,
-        the amount of possible combinations skyrockets. This is not a scalable solution to the problem.
-        
-        Object Extensions is an elegant way to handle scenarios such as this one. Rather than creating a new subclass for each possible combination,
-        you create one extension representing each feature. When you need to create a car with a particular set of features,
-        you take the parent class and pass it the exact set of extensions you want to apply via the `.with_extensions()` method as the need arises.
-        
-        Note that this pattern is intended to be used alongside inheritance, not to replace it entirely. The two can be mixed without issue, such that
-        (for example) a subclass could extend a parent class that has pre-applied extensions like so:
-        ```python
-        class SpecificCarModel(Car.with_extensions(TouchscreenDash)):
-            pass
-        ```
-        
-        ## Quickstart
-        
-        ### Setup
-        
-        Below is an example of an extendable class, and an example extension that can be applied to it.
-        
-        ```python
-        from objectextensions import Extendable
-        
-        
-        class HashList(Extendable):
-            """
-            A basic example class with some data and methods.
-            Inheriting Extendable allows this class to be modified with extensions
-            """
-        
-            def __init__(self, iterable=()):
-                super().__init__()
-        
-                self.values = {}
-                self.list = []
-        
-                for value in iterable:
-                    self.append(value)
-        
-            def append(self, item):
-                self.list.append(item)
-                self.values[item] = self.values.get(item, []) + [len(self.list) - 1]
-        
-            def index(self, item):
-                """
-                Returns all indexes containing the specified item.
-                Much lower time complexity than in a typical list due to dict lookup usage
-                """
-        
-                if item not in self.values:
-                    raise ValueError(f"{item} is not in hashlist")
-        
-                return self.values[item]
-        ```
-        ```python
-        from objectextensions import Extension
-        
-        
-        class Listener(Extension):
-            """
-            This extension class is written to apply a counter to the HashList class,
-            which increments any time .append() is called
-            """
-        
-            @staticmethod
-            def can_extend(target_cls):
-                return issubclass(target_cls, HashList)
-        
-            @staticmethod
-            def extend(target_cls):
-                Extension._set(target_cls, "increment_append_count", Listener.__increment_append_count)
-        
-                Extension._wrap(target_cls, "__init__", Listener.__wrap_init)
-                Extension._wrap(target_cls, 'append', Listener.__wrap_append)
-        
-            def __wrap_init(self, *args, **kwargs):
-                Extension._set(self, "append_count", 0)
-                yield
-        
-            def __wrap_append(self, *args, **kwargs):
-                yield
-                self.increment_append_count()
-        
-            def __increment_append_count(self):
-                self.append_count += 1
-        ```
-        
-        ### Instantiation
-        ```python
-        HashListWithListeners = HashList.with_extensions(Listener)
-        my_hashlist = HashListWithListeners(iterable=[5,2,4])
-        ```
-        or, for shorthand:
-        ```python
-        my_hashlist = HashList.with_extensions(Listener)(iterable=[5,2,4])
-        ```
-        
-        ### Result
-        ```python
-        >>> my_hashlist.append_count  # Attribute that was added by the Listener extension
-        3
-        >>> my_hashlist.append(7)  # Listener has wrapped this method with logic which increments .append_count
-        >>> my_hashlist.append_count
-        4
-        ```
-        
-        ## Functionality
-        
-        ### Properties
-        
-        Extendable.**extensions**  
-        &nbsp;&nbsp;&nbsp;&nbsp;Returns a reference to a tuple containing any applied extensions.  
-        &nbsp;
-        
-        Extendable.**extension_data**  
-        &nbsp;&nbsp;&nbsp;&nbsp;Returns a snapshot of the instance's extension data.  
-        &nbsp;&nbsp;&nbsp;&nbsp;This is intended to hold metadata optionally provided by extensions for the sake of introspection,  
-        &nbsp;&nbsp;&nbsp;&nbsp;and for communication between extensions.  
-        &nbsp;
-        
-        ### Methods
-        
-        Extendable.**with_extensions**(*cls, \*extensions: Type[Extension]*)  
-        &nbsp;&nbsp;&nbsp;&nbsp;Returns a subclass with the provided extensions applied to it.  
-        &nbsp;
-        
-        Extension.**can_extend**(*target_cls: Type[Extendable]*)  
-        &nbsp;&nbsp;&nbsp;&nbsp;Abstract staticmethod which must be overridden.  
-        &nbsp;&nbsp;&nbsp;&nbsp;Should return a bool indicating whether this Extension can be applied to the target class.  
-        &nbsp;
-        
-        Extension.**extend**(*target_cls: Type[Extendable]*)  
-        &nbsp;&nbsp;&nbsp;&nbsp;Abstract staticmethod which must be overridden.  
-        &nbsp;&nbsp;&nbsp;&nbsp;Any modification of the target class should take place in this function.  
-        &nbsp;
-        
-        Extension.**\_wrap**(*target_cls: Type[Extendable], method_name: str,*  
-        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*gen_func: Callable[..., Generator[None, Any, None]]*)  
-        &nbsp;&nbsp;&nbsp;&nbsp;Used to wrap an existing method on the target class.  
-        &nbsp;&nbsp;&nbsp;&nbsp;Passes copies of the method parameters to the generator function provided.  
-        &nbsp;&nbsp;&nbsp;&nbsp;The generator function should yield once,  
-        &nbsp;&nbsp;&nbsp;&nbsp;with the yield statement receiving a copy of the result of executing the core method.  
-        &nbsp;
-        
-        Extension.**\_set**(*target: Union[Type[Extendable], Extendable], attribute_name: str, value: Any*)  
-        &nbsp;&nbsp;&nbsp;&nbsp;Used to safely add a new attribute to an extendable class.  
-        
-        *Note: It is possible but not recommended to modify an instance rather than a class using this method.*  
-        &nbsp;&nbsp;&nbsp;&nbsp;*Will raise an error if the attribute already exists (for example, if another extension has already added it)*  
-        &nbsp;&nbsp;&nbsp;&nbsp;*to ensure compatibility issues are flagged and can be dealt with easily.*  
-        &nbsp;
-        
-        Extension.**\_set_property**(*target: Union[Type[Extendable], Extendable], property_name: str, value: Callable[[Extendable], Any]*)  
-        &nbsp;&nbsp;&nbsp;&nbsp;Used to safely add a new property to an extendable class.  
-        
-        *Note: It is possible but not recommended to modify an instance rather than a class using this method.*  
-        &nbsp;&nbsp;&nbsp;&nbsp;*Will raise an error if the attribute already exists (for example, if another extension has already added it)*  
-        &nbsp;&nbsp;&nbsp;&nbsp;*to ensure compatibility issues are flagged and can be dealt with easily.*  
-        &nbsp;
-        
-        Extension.**\_set_setter**(*target: Union[Type[Extendable], Extendable], setter_name: str, linked_property_name: str,*  
-        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*value: Callable[[Extendable, Any], Any]*)  
-        &nbsp;&nbsp;&nbsp;&nbsp;Used to safely add a new setter to an extendable class.  
-        
-        *Note: It is possible but not recommended to modify an instance rather than a class using this method.*  
-        &nbsp;&nbsp;&nbsp;&nbsp;*If the property this setter is paired with does not use the same attribute name,*  
-        &nbsp;&nbsp;&nbsp;&nbsp;*and the setter's name already exists on the class (for example, if another extension has already added it),*  
-        &nbsp;&nbsp;&nbsp;&nbsp;*an error will be raised. This is to ensure compatibility issues are flagged and can be dealt with easily.*  
-        &nbsp;
-        
-        ## Additional Info
-        
-        - As extensions do not properly invoke name mangling, adding private members via extensions is discouraged; doing so may lead to unintended behaviour.
-        Using protected members instead is encouraged, as name mangling does not come into play in this case.
-        
 Keywords: extensions,plugins
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
+# Object Extensions
+
+###### A basic framework for implementing an extension pattern
+
+## Summary
+
+The point of this framework is to provide a more modular alternative to object inheritance.
+
+**Consider the following use case:** You have an abstract class `Car` intended to represent a car, and need a pattern that allows you to *optionally* add more features.
+For example, you may want to add a convertible roof or a touchscreen on the dashboard, but these features will not necessarily be added to every subclass of `Car` you create.
+
+Applying standard OOP here means you would need to make a subclass every time a new combination of these optional features is needed.
+In the above case, you may need one subclass for a car with a convertible roof, one subclass for a car with a touchscreen, and one that has both features. As the amount of optional features increases,
+the amount of possible combinations skyrockets. This is not a scalable solution to the problem.
+
+Object Extensions is an elegant way to handle scenarios such as this one. Rather than creating a new subclass for each possible combination,
+you create one extension representing each feature. When you need to create a car with a particular set of features,
+you take the parent class and pass it the exact set of extensions you want to apply via the `.with_extensions()` method as the need arises.
+
+Note that this pattern is intended to be used alongside inheritance, not to replace it entirely. The two can be mixed without issue, such that
+(for example) a subclass could extend a parent class that has pre-applied extensions like so:
+```python
+class SpecificCarModel(Car.with_extensions(TouchscreenDash)):
+    pass
+```
+
+## Quickstart
+
+### Setup
+
+Below is an example of an extendable class, and an example extension that can be applied to it.
+
+```python
+from objectextensions import Extendable
+
+
+class HashList(Extendable):
+    """
+    A basic example class with some data and methods.
+    Inheriting Extendable allows this class to be modified with extensions
+    """
+
+    def __init__(self, iterable=()):
+        super().__init__()
+
+        self.values = {}
+        self.list = []
+
+        for value in iterable:
+            self.append(value)
+
+    def append(self, item):
+        self.list.append(item)
+        self.values[item] = self.values.get(item, []) + [len(self.list) - 1]
+
+    def index(self, item):
+        """
+        Returns all indexes containing the specified item.
+        Much lower time complexity than in a typical list due to dict lookup usage
+        """
+
+        if item not in self.values:
+            raise ValueError(f"{item} is not in hashlist")
+
+        return self.values[item]
+```
+```python
+from objectextensions import Extension
+
+
+class Listener(Extension):
+    """
+    This extension class is written to apply a counter to the HashList class,
+    which increments any time .append() is called
+    """
+
+    @staticmethod
+    def can_extend(target_cls):
+        return issubclass(target_cls, HashList)
+
+    @staticmethod
+    def extend(target_cls):
+        Extension._set(target_cls, "increment_append_count", Listener.__increment_append_count)
+
+        Extension._wrap(target_cls, "__init__", Listener.__wrap_init)
+        Extension._wrap(target_cls, 'append', Listener.__wrap_append)
+
+    def __wrap_init(self, *args, **kwargs):
+        Extension._set(self, "append_count", 0)
+        yield
+
+    def __wrap_append(self, *args, **kwargs):
+        yield
+        self.increment_append_count()
+
+    def __increment_append_count(self):
+        self.append_count += 1
+```
+
+### Instantiation
+```python
+HashListWithListeners = HashList.with_extensions(Listener)
+my_hashlist = HashListWithListeners(iterable=[5,2,4])
+```
+or, for shorthand:
+```python
+my_hashlist = HashList.with_extensions(Listener)(iterable=[5,2,4])
+```
+
+### Result
+```python
+>>> my_hashlist.append_count  # Attribute that was added by the Listener extension
+3
+>>> my_hashlist.append(7)  # Listener has wrapped this method with logic which increments .append_count
+>>> my_hashlist.append_count
+4
+```
+
+## Functionality
+
+### Properties
+
+Extendable.**extensions**  
+&nbsp;&nbsp;&nbsp;&nbsp;Returns a reference to a tuple containing any applied extensions.  
+&nbsp;
+
+Extendable.**extension_data**  
+&nbsp;&nbsp;&nbsp;&nbsp;Returns a snapshot of the instance's extension data.  
+&nbsp;&nbsp;&nbsp;&nbsp;This is intended to hold metadata optionally provided by extensions for the sake of introspection,  
+&nbsp;&nbsp;&nbsp;&nbsp;and for communication between extensions.  
+&nbsp;
+
+### Methods
+
+Extendable.**with_extensions**(*cls, \*extensions: Type[Extension]*)  
+&nbsp;&nbsp;&nbsp;&nbsp;Returns a subclass with the provided extensions applied to it.  
+&nbsp;
+
+Extension.**can_extend**(*target_cls: Type[Extendable]*)  
+&nbsp;&nbsp;&nbsp;&nbsp;Abstract staticmethod which must be overridden.  
+&nbsp;&nbsp;&nbsp;&nbsp;Should return a bool indicating whether this Extension can be applied to the target class.  
+&nbsp;
+
+Extension.**extend**(*target_cls: Type[Extendable]*)  
+&nbsp;&nbsp;&nbsp;&nbsp;Abstract staticmethod which must be overridden.  
+&nbsp;&nbsp;&nbsp;&nbsp;Any modification of the target class should take place in this function.  
+&nbsp;
+
+Extension.**\_wrap**(*target_cls: Type[Extendable], method_name: str,*  
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*gen_func: Callable[..., Generator[None, Any, None]]*)  
+&nbsp;&nbsp;&nbsp;&nbsp;Used to wrap an existing method on the target class.  
+&nbsp;&nbsp;&nbsp;&nbsp;Passes copies of the method parameters to the generator function provided.  
+&nbsp;&nbsp;&nbsp;&nbsp;The generator function should yield once,  
+&nbsp;&nbsp;&nbsp;&nbsp;with the yield statement receiving a copy of the result of executing the core method.  
+&nbsp;
+
+Extension.**\_set**(*target: Union[Type[Extendable], Extendable], attribute_name: str, value: Any*)  
+&nbsp;&nbsp;&nbsp;&nbsp;Used to safely add a new attribute to an extendable class.  
+
+*Note: It is possible but not recommended to modify an instance rather than a class using this method.*  
+&nbsp;&nbsp;&nbsp;&nbsp;*Will raise an error if the attribute already exists (for example, if another extension has already added it)*  
+&nbsp;&nbsp;&nbsp;&nbsp;*to ensure compatibility issues are flagged and can be dealt with easily.*  
+&nbsp;
+
+Extension.**\_set_property**(*target: Union[Type[Extendable], Extendable], property_name: str, value: Callable[[Extendable], Any]*)  
+&nbsp;&nbsp;&nbsp;&nbsp;Used to safely add a new property to an extendable class.  
+
+*Note: It is possible but not recommended to modify an instance rather than a class using this method.*  
+&nbsp;&nbsp;&nbsp;&nbsp;*Will raise an error if the attribute already exists (for example, if another extension has already added it)*  
+&nbsp;&nbsp;&nbsp;&nbsp;*to ensure compatibility issues are flagged and can be dealt with easily.*  
+&nbsp;
+
+Extension.**\_set_setter**(*target: Union[Type[Extendable], Extendable], setter_name: str, linked_property_name: str,*  
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*value: Callable[[Extendable, Any], Any]*)  
+&nbsp;&nbsp;&nbsp;&nbsp;Used to safely add a new setter to an extendable class.  
+
+*Note: It is possible but not recommended to modify an instance rather than a class using this method.*  
+&nbsp;&nbsp;&nbsp;&nbsp;*If the property this setter is paired with does not use the same attribute name,*  
+&nbsp;&nbsp;&nbsp;&nbsp;*and the setter's name already exists on the class (for example, if another extension has already added it),*  
+&nbsp;&nbsp;&nbsp;&nbsp;*an error will be raised. This is to ensure compatibility issues are flagged and can be dealt with easily.*  
+&nbsp;
+
+## Additional Info
+
+- As extensions do not properly invoke name mangling, adding private members via extensions is discouraged; doing so may lead to unintended behaviour.
+Using protected members instead is encouraged, as name mangling does not come into play in this case.
```

### Comparing `objectextensions-2.0.1/setup.py` & `objectextensions-2.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,28 +4,28 @@
     long_description = readme_file.read()
 
 setup(
     name="objectextensions",
     packages=[
         "objectextensions"
     ],
-    version="2.0.1",
+    version="2.0.2",
     license="MIT",
     description="A basic framework for implementing an extension pattern",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="immijimmi",
     author_email="immijimmi1@gmail.com",
     url="https://github.com/immijimmi/objectextensions",
-    download_url="https://github.com/immijimmi/objectextensions/archive/refs/tags/v2.0.1.tar.gz",
+    download_url="https://github.com/immijimmi/objectextensions/archive/refs/tags/v2.0.2.tar.gz",
     keywords=["extensions", "plugins"],
     install_requires=[
-        "wrapt~=1.11.2"
+        "wrapt~=1.15.0"
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

