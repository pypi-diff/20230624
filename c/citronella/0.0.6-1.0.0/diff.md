# Comparing `tmp/citronella-0.0.6.tar.gz` & `tmp/citronella-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citronella-0.0.6.tar", last modified: Mon May 15 17:01:54 2023, max compression
+gzip compressed data, was "citronella-1.0.0.tar", last modified: Sat Jun 24 06:23:33 2023, max compression
```

## Comparing `citronella-0.0.6.tar` & `citronella-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-05-15 17:01:54.140217 citronella-0.0.6/
--rw-r--r--   0 noodle    (1000) wheel      (998)     9586 2023-05-15 17:01:54.140217 citronella-0.0.6/PKG-INFO
--rw-r--r--   0 noodle    (1000) wheel      (998)     8748 2023-05-15 16:54:12.000000 citronella-0.0.6/README.md
--rw-r--r--   0 noodle    (1000) wheel      (998)       38 2023-05-15 17:01:54.140217 citronella-0.0.6/setup.cfg
--rw-r--r--   0 noodle    (1000) wheel      (998)     1257 2023-03-11 12:44:04.000000 citronella-0.0.6/setup.py
-drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-05-15 17:01:54.140217 citronella-0.0.6/src/
-drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-05-15 17:01:54.140217 citronella-0.0.6/src/citronella/
--rw-r--r--   0 noodle    (1000) wheel      (998)     1186 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/__init__.py
--rw-r--r--   0 noodle    (1000) wheel      (998)     1535 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/deprecated.py
--rw-r--r--   0 noodle    (1000) wheel      (998)     1426 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/logger.py
--rw-r--r--   0 noodle    (1000) wheel      (998)     2210 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/page_decorator.py
--rw-r--r--   0 noodle    (1000) wheel      (998)     1452 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/page_validator.py
--rw-r--r--   0 noodle    (1000) wheel      (998)     1119 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/placeholder_page.py
--rw-r--r--   0 noodle    (1000) wheel      (998)     1527 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/ui.py
--rw-r--r--   0 noodle    (1000) wheel      (998)     5136 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/web_page.py
--rw-r--r--   0 noodle    (1000) wheel      (998)     5419 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/web_ui.py
-drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-05-15 17:01:54.140217 citronella-0.0.6/src/citronella.egg-info/
--rw-r--r--   0 noodle    (1000) wheel      (998)     9586 2023-05-15 17:01:54.000000 citronella-0.0.6/src/citronella.egg-info/PKG-INFO
--rw-r--r--   0 noodle    (1000) wheel      (998)      491 2023-05-15 17:01:54.000000 citronella-0.0.6/src/citronella.egg-info/SOURCES.txt
--rw-r--r--   0 noodle    (1000) wheel      (998)        1 2023-05-15 17:01:54.000000 citronella-0.0.6/src/citronella.egg-info/dependency_links.txt
--rw-r--r--   0 noodle    (1000) wheel      (998)        9 2023-05-15 17:01:54.000000 citronella-0.0.6/src/citronella.egg-info/requires.txt
--rw-r--r--   0 noodle    (1000) wheel      (998)       11 2023-05-15 17:01:54.000000 citronella-0.0.6/src/citronella.egg-info/top_level.txt
-drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-05-15 17:01:54.140217 citronella-0.0.6/test/
--rw-r--r--   0 noodle    (1000) wheel      (998)     1900 2023-04-29 22:47:14.000000 citronella-0.0.6/test/test_navigation_menu.py
+drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-06-24 06:23:33.091658 citronella-1.0.0/
+-rw-r--r--   0 noodle    (1000) wheel      (998)     9534 2023-06-24 06:23:33.091658 citronella-1.0.0/PKG-INFO
+-rw-r--r--   0 noodle    (1000) wheel      (998)     8696 2023-06-24 06:20:17.000000 citronella-1.0.0/README.md
+-rw-r--r--   0 noodle    (1000) wheel      (998)       38 2023-06-24 06:23:33.091658 citronella-1.0.0/setup.cfg
+-rw-r--r--   0 noodle    (1000) wheel      (998)     1257 2023-06-24 06:21:22.000000 citronella-1.0.0/setup.py
+drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-06-24 06:23:33.088325 citronella-1.0.0/src/
+drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-06-24 06:23:33.091658 citronella-1.0.0/src/citronella/
+-rw-r--r--   0 noodle    (1000) wheel      (998)     1140 2023-06-24 05:12:15.000000 citronella-1.0.0/src/citronella/__init__.py
+-rw-r--r--   0 noodle    (1000) wheel      (998)     1535 2023-05-15 16:59:51.000000 citronella-1.0.0/src/citronella/deprecated.py
+-rw-r--r--   0 noodle    (1000) wheel      (998)     1426 2023-05-15 16:59:51.000000 citronella-1.0.0/src/citronella/logger.py
+-rw-r--r--   0 noodle    (1000) wheel      (998)     2210 2023-05-15 16:59:51.000000 citronella-1.0.0/src/citronella/page_decorator.py
+-rw-r--r--   0 noodle    (1000) wheel      (998)     1452 2023-05-15 16:59:51.000000 citronella-1.0.0/src/citronella/page_validator.py
+-rw-r--r--   0 noodle    (1000) wheel      (998)     1376 2023-06-24 05:14:00.000000 citronella-1.0.0/src/citronella/ui.py
+-rw-r--r--   0 noodle    (1000) wheel      (998)     3921 2023-06-24 06:08:54.000000 citronella-1.0.0/src/citronella/web_page.py
+-rw-r--r--   0 noodle    (1000) wheel      (998)     5049 2023-06-24 05:16:46.000000 citronella-1.0.0/src/citronella/web_ui.py
+drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-06-24 06:23:33.091658 citronella-1.0.0/src/citronella.egg-info/
+-rw-r--r--   0 noodle    (1000) wheel      (998)     9534 2023-06-24 06:23:33.000000 citronella-1.0.0/src/citronella.egg-info/PKG-INFO
+-rw-r--r--   0 noodle    (1000) wheel      (998)      456 2023-06-24 06:23:33.000000 citronella-1.0.0/src/citronella.egg-info/SOURCES.txt
+-rw-r--r--   0 noodle    (1000) wheel      (998)        1 2023-06-24 06:23:33.000000 citronella-1.0.0/src/citronella.egg-info/dependency_links.txt
+-rw-r--r--   0 noodle    (1000) wheel      (998)        9 2023-06-24 06:23:33.000000 citronella-1.0.0/src/citronella.egg-info/requires.txt
+-rw-r--r--   0 noodle    (1000) wheel      (998)       11 2023-06-24 06:23:33.000000 citronella-1.0.0/src/citronella.egg-info/top_level.txt
+drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-06-24 06:23:33.091658 citronella-1.0.0/test/
+-rw-r--r--   0 noodle    (1000) wheel      (998)     2082 2023-06-24 05:46:15.000000 citronella-1.0.0/test/test_navigation_menu.py
```

### Comparing `citronella-0.0.6/PKG-INFO` & `citronella-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citronella
-Version: 0.0.6
+Version: 1.0.0
 Summary: Webdriver Extension with Page Object Wrapper
 Home-page: https://github.com/heyclore/citronella/tree/main/python#readme
 Author: heyclore
 Author-email: cloore@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/heyclore/citronella/tree/main/python
 Keywords: test,unittest,pytest,webdriver,appium,selenium
@@ -152,18 +152,18 @@
 * The second module are for the page object model.
 
 ### Selenium
 
 ```python
 from selenium.webdriver.common.by import By
 from citronella import ui
-from Pages.contents_page import ContentsPage
+from Pages.components import Header
 
 
-class HomePage(ContentsPage().header()):
+class HomePage(Header):
 
     def some_button(self):
         return ui(By.XPATH, '//a[@name="foo"]')
 
     def search_input(self):
         return ui(By.ID, 'search')
 
@@ -172,18 +172,18 @@
 ```
 
 ### Appium
 
 ```python
 from appium.webdriver.common.appiumby import AppiumBy
 from citronella import ui
-from Pages.contents_page import ContentsPage
+from Pages.components import Header
 
 
-class HomePage(ContentsPage().header()):
+class HomePage(Header):
 
     def some_button(self):
         return ui(AppiumBy.XPATH, '//a[@name="foo"]')
 
     def search_input(self):
         return ui(AppiumBy.ACCESSIBILITY_ID, 'search')
```

### Comparing `citronella-0.0.6/README.md` & `citronella-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -131,18 +131,18 @@
 * The second module are for the page object model.
 
 ### Selenium
 
 ```python
 from selenium.webdriver.common.by import By
 from citronella import ui
-from Pages.contents_page import ContentsPage
+from Pages.components import Header
 
 
-class HomePage(ContentsPage().header()):
+class HomePage(Header):
 
     def some_button(self):
         return ui(By.XPATH, '//a[@name="foo"]')
 
     def search_input(self):
         return ui(By.ID, 'search')
 
@@ -151,18 +151,18 @@
 ```
 
 ### Appium
 
 ```python
 from appium.webdriver.common.appiumby import AppiumBy
 from citronella import ui
-from Pages.contents_page import ContentsPage
+from Pages.components import Header
 
 
-class HomePage(ContentsPage().header()):
+class HomePage(Header):
 
     def some_button(self):
         return ui(AppiumBy.XPATH, '//a[@name="foo"]')
 
     def search_input(self):
         return ui(AppiumBy.ACCESSIBILITY_ID, 'search')
```

### Comparing `citronella-0.0.6/setup.py` & `citronella-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="citronella",
-    version="0.0.6",
+    version="1.0.0",
     license="MIT",
     description="Webdriver Extension with Page Object Wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/heyclore/citronella/tree/main/python#readme",
     author="heyclore",
     author_email="cloore@gmail.com",
```

### Comparing `citronella-0.0.6/src/citronella/__init__.py` & `citronella-1.0.0/src/citronella/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,8 +19,7 @@
 #LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #SOFTWARE.
 
 
 from .ui import ui
 from .web_page import WebPage
-from .placeholder_page import PlaceholderPage
```

### Comparing `citronella-0.0.6/src/citronella/deprecated.py` & `citronella-1.0.0/src/citronella/deprecated.py`

 * *Files identical despite different names*

### Comparing `citronella-0.0.6/src/citronella/logger.py` & `citronella-1.0.0/src/citronella/logger.py`

 * *Files identical despite different names*

### Comparing `citronella-0.0.6/src/citronella/page_decorator.py` & `citronella-1.0.0/src/citronella/page_decorator.py`

 * *Files identical despite different names*

### Comparing `citronella-0.0.6/src/citronella/page_validator.py` & `citronella-1.0.0/src/citronella/page_validator.py`

 * *Files identical despite different names*

### Comparing `citronella-0.0.6/src/citronella/placeholder_page.py` & `citronella-1.0.0/src/citronella/ui.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,8 +17,25 @@
 #FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #SOFTWARE.
 
 
-class PlaceholderPage: pass
+from .deprecated import logwarning
+
+
+def ui(by, value):
+    """
+    forward the data to page decorator and wrap into WebUi class.
+
+    Args:
+        by
+        ui
+
+    Usage:
+        ui(By.NAME, 'q')
+    """
+    return {
+            'by': by,
+            'value': value,
+            }
```

### Comparing `citronella-0.0.6/src/citronella/web_page.py` & `citronella-1.0.0/src/citronella/web_page.py`

 * *Files 23% similar despite different names*

```diff
@@ -58,31 +58,14 @@
         self._logger = logger
 
     @property
     def driver(self):
         """return the original selenium / appium driver."""
         return self._driver
 
-    ##
-    def page_object(self, new_page, get_start=False):
-        """
-        initialize page object module object.
-
-        Args:
-            page_object_model
-
-        Usage:
-            web.page_object(ContentsPage)
-        """
-        self._contents_page = new_page
-        logwarning('\n\t "page_object" method is deprecated and will remove for the next version'
-                   '\n\t use "web.page = HomePage" instead \n\t or \n\t "web.page = ContentsPage"'
-                   )
-    ##
-
     @property
     def page(self):
         """return a page decorator object of ContentsPage."""
         if not self._contents_page:
             warning('\n\tpage object hasn\'t been set yet.'
                     '\n\t"web = WebPage(driver, contents_page=ContentsPage)" '
                     'before "using web.page.foo.click()" etc.')
@@ -105,37 +88,15 @@
 
         Usage:
             web.locate(By.NAME, 'q').ec_presence_of_element_located()
             web.locate(By.NAME, 'q').get_element().text()
             web.locate(By.NAME, 'q').get_element().click()
         """
         return WebUi(self._driver, self._webdriver_wait, self._logger, by,
-                     value, self.locate.__name__, self.__class__.__name__)
-
-    ##
-    @property
-    def back(self):
-        """return to previous page."""
-        self.driver.back()
-        logwarning('"back" method is deprecated and will remove for the next '
-                   'version.\n\t use "web.driver.back()" instead.')
-
-    @property
-    def get_window_size(self):
-        """
-        get current windows size.
-
-        Usage:
-            height = web.get_window_size.height
-            width = web.get_window_size.width
-        """
-        logwarning('"get_window_size" method is deprecated and will remove for the next '
-                   'version.\n\t use "web.driver.get_window_size()" instead.')
-        return SimpleNamespace(**self.driver.get_window_size())
-    ##
+                     value, f'{by}: {value}', self.locate.__name__)
 
     def ready_state(self, timeout=30):
         """execute javascript for page to fully load"""
         for x in range(timeout):
             if self.driver.execute_script(
                     'return document.readyState') != 'complete':
                 sleep(1)
```

### Comparing `citronella-0.0.6/src/citronella/web_ui.py` & `citronella-1.0.0/src/citronella/web_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,35 +106,25 @@
     @logger
     def get_elements(self):
         """return list of web element, equal as find_elements."""
         return self._webdriver_wait(presence_of_all_elements_located(
             self._locator))
 
     @logger
-    def click(self, switch_page=True):
+    def click(self):
         """click to web element."""
-        ##
-        if not switch_page:
-            logwarning('"switch_page" kwargs is deprecated and will remove for the next version')
-            return
-        ##
         try:
             self._webdriver_wait(element_to_be_clickable(self._locator)).click()
         except Exception as e:
             sleep(2)
             self._webdriver_wait(element_to_be_clickable(self._locator)).click()
 
     @logger
-    def send_keys(self, text, clear=False, return_key=False, switch_page=True):
+    def send_keys(self, text, clear=False, return_key=False):
         """custom webdriver send_keys with optional clear field."""
-        ##
-        if not switch_page:
-            logwarning('"switch_page" kwargs is deprecated and will remove for the next version')
-            return
-        ##
         element = self._webdriver_wait(presence_of_element_located(self._locator))
 
         if clear:
             element.clear()
 
         element.send_keys(text)
```

### Comparing `citronella-0.0.6/src/citronella.egg-info/PKG-INFO` & `citronella-1.0.0/src/citronella.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citronella
-Version: 0.0.6
+Version: 1.0.0
 Summary: Webdriver Extension with Page Object Wrapper
 Home-page: https://github.com/heyclore/citronella/tree/main/python#readme
 Author: heyclore
 Author-email: cloore@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/heyclore/citronella/tree/main/python
 Keywords: test,unittest,pytest,webdriver,appium,selenium
@@ -152,18 +152,18 @@
 * The second module are for the page object model.
 
 ### Selenium
 
 ```python
 from selenium.webdriver.common.by import By
 from citronella import ui
-from Pages.contents_page import ContentsPage
+from Pages.components import Header
 
 
-class HomePage(ContentsPage().header()):
+class HomePage(Header):
 
     def some_button(self):
         return ui(By.XPATH, '//a[@name="foo"]')
 
     def search_input(self):
         return ui(By.ID, 'search')
 
@@ -172,18 +172,18 @@
 ```
 
 ### Appium
 
 ```python
 from appium.webdriver.common.appiumby import AppiumBy
 from citronella import ui
-from Pages.contents_page import ContentsPage
+from Pages.components import Header
 
 
-class HomePage(ContentsPage().header()):
+class HomePage(Header):
 
     def some_button(self):
         return ui(AppiumBy.XPATH, '//a[@name="foo"]')
 
     def search_input(self):
         return ui(AppiumBy.ACCESSIBILITY_ID, 'search')
```

### Comparing `citronella-0.0.6/test/test_navigation_menu.py` & `citronella-1.0.0/test/test_navigation_menu.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import pytest
-from Pages.home.home_page import HomePage
+from Pages.contents_page import ContentsPage
 from selenium.webdriver.common.by import By
 
 
 class TestNavigationMenu:
 
     def test_help_page(self, web):
         web.driver.get('https://pypi.org/')
-        web.page_object(HomePage)
-        web.ready_state_toggle
+        web.page = ContentsPage
 
-        web.page.help_button.click()
+        web.page.home_page.help_button.click()
         assert 'Help' in web.driver.title
 
     def test_sponsors_page(self, web):
-        web.page.sponsors_button.click()
+        web.page.help_page.sponsors_button.click()
         assert 'Sponsors' in web.driver.title
 
     def test_login_page(self, web):
-        web.page.login_button.click()
+        web.page.sponsors_page.login_button.click()
         assert 'Log' in web.driver.title
 
     def test_register_page(self, web):
-        web.page.register_button.click()
+        web.page.login_page.register_button.click()
         assert 'Create' in web.driver.title
 
     def test_foo_bar_baz(self, web):
-        web.page.register_button.ec_element_to_be_clickable()
-        web.page.register_button.ec_presence_of_element_located()
-        web.page.register_button.ec_presence_of_all_elements_located()
-        web.page.register_button.ec_visibility_of_element_located()
-        web.page.register_button.ec_visibility_of_all_elements_located()
-        web.page.register_button.ec_visibility_of_any_elements_located()
-        #web.page.register_button.ec_element_located_to_be_selected()
-        #web.page.register_button.ec_invisibility_of_element_located()
+        web.page.register_page.register_button.ec_element_to_be_clickable()
+        web.page.register_page.register_button.ec_presence_of_element_located()
+        web.page.register_page.register_button.ec_presence_of_all_elements_located()
+        web.page.register_page.register_button.ec_visibility_of_element_located()
+        web.page.register_page.register_button.ec_visibility_of_all_elements_located()
+        web.page.register_page.register_button.ec_visibility_of_any_elements_located()
+        #web.page.register_page.register_button.ec_element_located_to_be_selected()
+        #web.page.register_page.register_button.ec_invisibility_of_element_located()
 
     def test_locate(self, web):
         web.locate(By.ID, 'search').send_keys('citrone')
         web.locate(By.XPATH, '//button[@type="submit"]/i').click()
         assert 'citronella' in [x.text for x in web.locate(By.XPATH,
         '//span[@class="package-snippet__name"]').get_elements()]
 
     def test_search_package(self, web):
-        web.page.search_input.send_keys('citronella', return_key=True, clear=True)
-        result = web.page.search_lists_result.get_elements()
+        web.page.register_page.search_input.send_keys(
+                'citronella', return_key=True, clear=True)
+        result = web.page.search_page.search_lists_result.get_elements()
         assert 'citronella' in [
-                x.text for x in web.page.search_lists_result.get_elements()]
+                x.text for x in web.page.search_page.search_lists_result.get_elements()]
```

