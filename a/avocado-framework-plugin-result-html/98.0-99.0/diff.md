# Comparing `tmp/avocado-framework-plugin-result-html-98.0.tar.gz` & `tmp/avocado-framework-plugin-result-html-99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avocado-framework-plugin-result-html-98.0.tar", last modified: Thu Jul 14 20:53:55 2022, max compression
+gzip compressed data, was "avocado-framework-plugin-result-html-99.0.tar", last modified: Thu Nov 10 19:12:52 2022, max compression
```

## Comparing `avocado-framework-plugin-result-html-98.0.tar` & `avocado-framework-plugin-result-html-99.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:55.109647 avocado-framework-plugin-result-html-98.0/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       65 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-98.0/MANIFEST.in
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      230 2022-07-14 20:53:55.108647 avocado-framework-plugin-result-html-98.0/PKG-INFO
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        5 2022-07-14 20:50:57.000000 avocado-framework-plugin-result-html-98.0/VERSION
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:55.106647 avocado-framework-plugin-result-html-98.0/avocado_framework_plugin_result_html.egg-info/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      230 2022-07-14 20:53:55.000000 avocado-framework-plugin-result-html-98.0/avocado_framework_plugin_result_html.egg-info/PKG-INFO
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      989 2022-07-14 20:53:55.000000 avocado-framework-plugin-result-html-98.0/avocado_framework_plugin_result_html.egg-info/SOURCES.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        1 2022-07-14 20:53:55.000000 avocado-framework-plugin-result-html-98.0/avocado_framework_plugin_result_html.egg-info/dependency_links.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      178 2022-07-14 20:53:55.000000 avocado-framework-plugin-result-html-98.0/avocado_framework_plugin_result_html.egg-info/entry_points.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       31 2022-07-14 20:53:55.000000 avocado-framework-plugin-result-html-98.0/avocado_framework_plugin_result_html.egg-info/requires.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       26 2022-07-14 20:53:55.000000 avocado-framework-plugin-result-html-98.0/avocado_framework_plugin_result_html.egg-info/top_level.txt
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:55.107647 avocado-framework-plugin-result-html-98.0/avocado_result_html/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    11920 2022-07-11 13:32:25.000000 avocado-framework-plugin-result-html-98.0/avocado_result_html/__init__.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:55.108647 avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5925 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/avocado_html.js
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    49657 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/bootstrap.min.css
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    16595 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/bootstrap.min.js
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5245 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/datatables.bootstrap.js
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    12525 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/datatables.css
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    79972 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/datatables.min.js
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:55.108647 avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/images/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     9784 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/images/logs_icon.svg
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3258 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/images/whiteboard_icon.svg
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    93196 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/jquery.min.js
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    11155 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/results.html
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1376 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/style.css
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       38 2022-07-14 20:53:55.109647 avocado-framework-plugin-result-html-98.0/setup.cfg
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1366 2022-07-11 13:32:25.000000 avocado-framework-plugin-result-html-98.0/setup.py
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:53:55.108647 avocado-framework-plugin-result-html-98.0/tests/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-03-14 18:04:28.000000 avocado-framework-plugin-result-html-98.0/tests/__init__.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4520 2022-07-11 13:32:25.000000 avocado-framework-plugin-result-html-98.0/tests/test_html_result.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:52.934180 avocado-framework-plugin-result-html-99.0/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       65 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-99.0/MANIFEST.in
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      230 2022-11-10 19:12:52.934180 avocado-framework-plugin-result-html-99.0/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        5 2022-11-10 19:09:51.000000 avocado-framework-plugin-result-html-99.0/VERSION
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:52.932181 avocado-framework-plugin-result-html-99.0/avocado_framework_plugin_result_html.egg-info/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      230 2022-11-10 19:12:52.000000 avocado-framework-plugin-result-html-99.0/avocado_framework_plugin_result_html.egg-info/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      989 2022-11-10 19:12:52.000000 avocado-framework-plugin-result-html-99.0/avocado_framework_plugin_result_html.egg-info/SOURCES.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        1 2022-11-10 19:12:52.000000 avocado-framework-plugin-result-html-99.0/avocado_framework_plugin_result_html.egg-info/dependency_links.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      178 2022-11-10 19:12:52.000000 avocado-framework-plugin-result-html-99.0/avocado_framework_plugin_result_html.egg-info/entry_points.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       31 2022-11-10 19:12:52.000000 avocado-framework-plugin-result-html-99.0/avocado_framework_plugin_result_html.egg-info/requires.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       26 2022-11-10 19:12:52.000000 avocado-framework-plugin-result-html-99.0/avocado_framework_plugin_result_html.egg-info/top_level.txt
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:52.932181 avocado-framework-plugin-result-html-99.0/avocado_result_html/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    11920 2022-11-04 17:27:10.000000 avocado-framework-plugin-result-html-99.0/avocado_result_html/__init__.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:52.933180 avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5928 2022-11-04 17:27:10.000000 avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/avocado_html.js
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)    49657 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/bootstrap.min.css
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)    16595 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/bootstrap.min.js
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)     5245 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/datatables.bootstrap.js
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)    12525 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/datatables.css
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)    79972 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/datatables.min.js
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:52.934180 avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/images/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)     9784 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/images/logs_icon.svg
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)     3258 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/images/whiteboard_icon.svg
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)    93196 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/jquery.min.js
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)    11155 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/results.html
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)     1376 2021-05-24 13:07:35.000000 avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/style.css
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       38 2022-11-10 19:12:52.934180 avocado-framework-plugin-result-html-99.0/setup.cfg
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1366 2022-11-04 17:27:10.000000 avocado-framework-plugin-result-html-99.0/setup.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:52.934180 avocado-framework-plugin-result-html-99.0/tests/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)        0 2022-03-14 18:04:28.000000 avocado-framework-plugin-result-html-99.0/tests/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4520 2022-11-04 17:27:10.000000 avocado-framework-plugin-result-html-99.0/tests/test_html_result.py
```

### Comparing `avocado-framework-plugin-result-html-98.0/avocado_framework_plugin_result_html.egg-info/SOURCES.txt` & `avocado-framework-plugin-result-html-99.0/avocado_framework_plugin_result_html.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-result-html-98.0/avocado_result_html/__init__.py` & `avocado-framework-plugin-result-html-99.0/avocado_result_html/__init__.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/avocado_html.js` & `avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/avocado_html.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -12,15 +12,15 @@
             drawCallback: onTableRedrawn.bind(null, resizeControl),
             initComplete: onDatatablesInitialized
         });
     });
 
     function onDatatablesInitialized() {
         var statusColumn = this.api().column(4);
-        var select = $('<select class="form-control input-sm"><option value=""></option></select>')
+        var select = $('<select class="form-control input-sm"><option value="">ALL</option></select>')
             .on('change', function() {
                 var val = $(this).val()
                 statusColumn.search(val ? '^' + val + '$' : '', true, false).draw();
             });
 
         $('#results_length').wrap('<div class="row"><div class="col-sm-4"></div></div>');
         $('#results_length').parent().parent()
```

### Comparing `avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/bootstrap.min.css` & `avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/bootstrap.min.js` & `avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/datatables.bootstrap.js` & `avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/datatables.bootstrap.js`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/datatables.css` & `avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/datatables.css`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/datatables.min.js` & `avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/datatables.min.js`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/images/logs_icon.svg` & `avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/images/logs_icon.svg`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/images/whiteboard_icon.svg` & `avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/images/whiteboard_icon.svg`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/jquery.min.js` & `avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/jquery.min.js`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/results.html` & `avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/results.html`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-result-html-98.0/avocado_result_html/templates/style.css` & `avocado-framework-plugin-result-html-99.0/avocado_result_html/templates/style.css`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-result-html-98.0/setup.py` & `avocado-framework-plugin-result-html-99.0/setup.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-result-html-98.0/tests/test_html_result.py` & `avocado-framework-plugin-result-html-99.0/tests/test_html_result.py`

 * *Files identical despite different names*

