# Comparing `tmp/masterqa-1.8.3.tar.gz` & `tmp/masterqa-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masterqa-1.8.3.tar", last modified: Wed Jun 14 00:35:52 2023, max compression
+gzip compressed data, was "masterqa-1.8.4.tar", last modified: Sat Jun 24 20:38:49 2023, max compression
```

## Comparing `masterqa-1.8.3.tar` & `masterqa-1.8.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-14 00:35:52.376828 masterqa-1.8.3/
--rw-r--r--   0 michael    (501) staff       (20)     1682 2022-12-06 03:15:26.000000 masterqa-1.8.3/.gitignore
--rw-r--r--   0 michael    (501) staff       (20)     1080 2022-12-06 03:15:26.000000 masterqa-1.8.3/LICENSE
--rw-r--r--   0 michael    (501) staff       (20)      100 2022-12-06 03:15:26.000000 masterqa-1.8.3/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     3015 2023-06-14 00:35:52.376898 masterqa-1.8.3/PKG-INFO
--rwxr-xr-x   0 michael    (501) staff       (20)     2616 2023-01-24 04:43:53.000000 masterqa-1.8.3/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-14 00:35:52.375926 masterqa-1.8.3/masterqa/
--rwxr-xr-x   0 michael    (501) staff       (20)       48 2022-12-06 03:15:26.000000 masterqa-1.8.3/masterqa/__init__.py
--rwxr-xr-x   0 michael    (501) staff       (20)    17697 2023-04-21 19:32:04.000000 masterqa-1.8.3/masterqa/master_qa.py
--rwxr-xr-x   0 michael    (501) staff       (20)      718 2022-12-06 03:15:26.000000 masterqa-1.8.3/masterqa/settings.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-14 00:35:52.376696 masterqa-1.8.3/masterqa.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     3015 2023-06-14 00:35:52.000000 masterqa-1.8.3/masterqa.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      310 2023-06-14 00:35:52.000000 masterqa-1.8.3/masterqa.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-14 00:35:52.000000 masterqa-1.8.3/masterqa.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       77 2023-06-14 00:35:52.000000 masterqa-1.8.3/masterqa.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        9 2023-06-14 00:35:52.000000 masterqa-1.8.3/masterqa.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)     1440 2023-04-21 19:32:04.000000 masterqa-1.8.3/pytest.ini
--rwxr-xr-x   0 michael    (501) staff       (20)       82 2023-06-14 00:32:16.000000 masterqa-1.8.3/requirements.txt
--rwxr-xr-x   0 michael    (501) staff       (20)      188 2023-06-14 00:35:52.377138 masterqa-1.8.3/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     3481 2023-06-14 00:32:16.000000 masterqa-1.8.3/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-24 20:38:49.201899 masterqa-1.8.4/
+-rw-r--r--   0 michael    (501) staff       (20)     1682 2022-12-06 03:15:26.000000 masterqa-1.8.4/.gitignore
+-rw-r--r--   0 michael    (501) staff       (20)     1080 2022-12-06 03:15:26.000000 masterqa-1.8.4/LICENSE
+-rw-r--r--   0 michael    (501) staff       (20)      100 2022-12-06 03:15:26.000000 masterqa-1.8.4/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)     3015 2023-06-24 20:38:49.201947 masterqa-1.8.4/PKG-INFO
+-rwxr-xr-x   0 michael    (501) staff       (20)     2616 2023-01-24 04:43:53.000000 masterqa-1.8.4/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-24 20:38:49.201285 masterqa-1.8.4/masterqa/
+-rwxr-xr-x   0 michael    (501) staff       (20)       48 2022-12-06 03:15:26.000000 masterqa-1.8.4/masterqa/__init__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    17607 2023-06-24 20:37:34.000000 masterqa-1.8.4/masterqa/master_qa.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      718 2022-12-06 03:15:26.000000 masterqa-1.8.4/masterqa/settings.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-24 20:38:49.201789 masterqa-1.8.4/masterqa.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     3015 2023-06-24 20:38:49.000000 masterqa-1.8.4/masterqa.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      310 2023-06-24 20:38:49.000000 masterqa-1.8.4/masterqa.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-24 20:38:49.000000 masterqa-1.8.4/masterqa.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       77 2023-06-24 20:38:49.000000 masterqa-1.8.4/masterqa.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        9 2023-06-24 20:38:49.000000 masterqa-1.8.4/masterqa.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1440 2023-04-21 19:32:04.000000 masterqa-1.8.4/pytest.ini
+-rwxr-xr-x   0 michael    (501) staff       (20)       82 2023-06-24 20:37:34.000000 masterqa-1.8.4/requirements.txt
+-rwxr-xr-x   0 michael    (501) staff       (20)      188 2023-06-24 20:38:49.202131 masterqa-1.8.4/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     3643 2023-06-24 20:37:34.000000 masterqa-1.8.4/setup.py
```

### Comparing `masterqa-1.8.3/.gitignore` & `masterqa-1.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `masterqa-1.8.3/LICENSE` & `masterqa-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `masterqa-1.8.3/PKG-INFO` & `masterqa-1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterqa
-Version: 1.8.3
+Version: 1.8.4
 Summary: Automation-Assisted Manual Testing - https://masterqa.com
 Home-page: https://github.com/masterqa/MasterQA
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Platform: Windows
```

### Comparing `masterqa-1.8.3/README.md` & `masterqa-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `masterqa-1.8.3/masterqa/master_qa.py` & `masterqa-1.8.4/masterqa/master_qa.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,54 +56,56 @@
                 f == RESULTS_PAGE) or (f.startswith("automation_failure")) or (
                 f == BAD_PAGE_LOG)]
             for f in filelist:
                 os.remove("%s/%s" % (file_path, f))
 
     def jq_confirm_dialog(self, question):
         count = self.manual_check_count + 1
-        title_content = ('<center><font color="#7700bb">Manual Check #%s:'
-                         '</font></center><hr><font color="#0066ff">%s</font>'
-                         '' % (count, question))
+        title_content = (
+            '<center><font color="#7700bb">Manual Check #%s:'
+            '</font></center><hr><font color="#0066ff">%s</font>'
+            '' % (count, question)
+        )
         title_content = js_utils.escape_quotes_if_needed(title_content)
         jqcd = (
             """jconfirm({
-                    boxWidth: '32.5%%',
-                    useBootstrap: false,
-                    containerFluid: false,
-                    animationBounce: 1,
-                    type: 'default',
-                    theme: 'bootstrap',
-                    typeAnimated: true,
-                    animation: 'scale',
-                    draggable: true,
-                    dragWindowGap: 1,
-                    container: 'body',
-                    title: '%s',
-                    content: '',
-                    buttons: {
-                        pass_button: {
-                            btnClass: 'btn-green',
-                            text: 'YES / PASS',
-                            keys: ['y', 'p', '1'],
-                            action: function(){
-                                $jqc_status = "Success!";
-                                jconfirm.lastButtonText = "Success!";
-                            }
-                        },
-                        fail_button: {
-                            btnClass: 'btn-red',
-                            text: 'NO / FAIL',
-                            keys: ['n', 'f', '2'],
-                            action: function(){
-                                $jqc_status = "Failure!";
-                                jconfirm.lastButtonText = "Failure!";
-                            }
+                boxWidth: '32.5%%',
+                useBootstrap: false,
+                containerFluid: false,
+                animationBounce: 1,
+                type: 'default',
+                theme: 'bootstrap',
+                typeAnimated: true,
+                animation: 'scale',
+                draggable: true,
+                dragWindowGap: 1,
+                container: 'body',
+                title: '%s',
+                content: '',
+                buttons: {
+                    pass_button: {
+                        btnClass: 'btn-green',
+                        text: 'YES / PASS',
+                        keys: ['y', 'p', '1'],
+                        action: function(){
+                            $jqc_status = "Success!";
+                            jconfirm.lastButtonText = "Success!";
+                        }
+                    },
+                    fail_button: {
+                        btnClass: 'btn-red',
+                        text: 'NO / FAIL',
+                        keys: ['n', 'f', '2'],
+                        action: function(){
+                            $jqc_status = "Failure!";
+                            jconfirm.lastButtonText = "Failure!";
                         }
                     }
-                });"""
+                }
+            });"""
             % title_content
         )
         self.execute_script(jqcd)
 
     def manual_page_check(self, *args):
         if not args:
             instructions = DEFAULT_VALIDATION_MESSAGE  # self.verify()
@@ -199,29 +201,33 @@
                     self.manual_check_count,
                     "Success",
                     "-",
                     current_url,
                     self.browser,
                     self.get_timestamp()[:-3],
                     instructions,
-                    "*"))
+                    "*",
+                )
+            )
             return 1
         else:
             bad_page_name = "failed_check_%s.png" % self.manual_check_count
             self.save_screenshot(bad_page_name, folder=LATEST_REPORT_DIR)
             self.page_results_list.append(
                 '"%s","%s","%s","%s","%s","%s","%s","%s"' % (
                     self.manual_check_count,
                     "FAILED!",
                     bad_page_name,
                     current_url,
                     self.browser,
                     self.get_timestamp()[:-3],
                     instructions,
-                    "*"))
+                    "*",
+                )
+            )
             return 0
 
     def wait_for_special_alert_absent(self, timeout=MAX_IDLE_TIME_BEFORE_QUIT):
         for x in range(int(timeout * 20)):
             try:
                 alert = self.driver.switch_to.alert
                 dummy_variable = alert.text  # Raises exception if no alert
@@ -252,15 +258,17 @@
                 "ERR",
                 "ERROR!",
                 error_page,
                 self.driver.current_url,
                 self.browser,
                 self.get_timestamp()[:-3],
                 "-",
-                exc_info))
+                exc_info,
+            )
+        )
         try:
             # Return to the original window if another was opened
             self.driver.switch_to_window(self.driver.window_handles[1])
             self.driver.close()
             self.driver.switch_to_window(self.driver.window_handles[0])
         except Exception:
             pass
@@ -322,43 +330,50 @@
         if failures_count > 0:
             tf_color = "#EE3A3A"
 
         ir_color = "#11BB11"
         if self.incomplete_runs > 0:
             ir_color = "#EE3A3A"
 
-        summary_table = '''<div><table><thead><tr>
-              <th>TESTING SUMMARY</th>
-              <th>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</th>
-              </tr></thead><tbody>
-              <tr style="color:#00BB00"><td>CHECKS PASSED: <td>%s</tr>
-              <tr style="color:%s"     ><td>CHECKS FAILED: <td>%s</tr>
-              <tr style="color:#4D4DDD"><td>TOTAL VERIFICATIONS: <td>%s</tr>
-              <tr style="color:%s"     ><td>INCOMPLETE TEST RUNS: <td>%s</tr>
-              </tbody></table>''' % (self.manual_check_successes,
-                                     tf_color,
-                                     failures_count,
-                                     self.manual_check_count,
-                                     ir_color,
-                                     self.incomplete_runs)
+        summary_table = (
+            '''<div><table><thead><tr>
+            <th>TESTING SUMMARY</th>
+            <th>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</th>
+            </tr></thead><tbody>
+            <tr style="color:#00BB00"><td>CHECKS PASSED: <td>%s</tr>
+            <tr style="color:%s"     ><td>CHECKS FAILED: <td>%s</tr>
+            <tr style="color:#4D4DDD"><td>TOTAL VERIFICATIONS: <td>%s</tr>
+            <tr style="color:%s"     ><td>INCOMPLETE TEST RUNS: <td>%s</tr>
+            </tbody></table>''' % (
+                self.manual_check_successes,
+                tf_color,
+                failures_count,
+                self.manual_check_count,
+                ir_color,
+                self.incomplete_runs,
+            )
+        )
 
         summary_table = (
             '''<h1 id="ContextHeader" class="sectionHeader" title="">
             %s</h1>''' % summary_table
         )
 
         log_link_shown = '../%s%s/' % (
             ARCHIVE_DIR, web_log_path.split(ARCHIVE_DIR)[1])
         csv_link = '%s/%s' % (web_log_path, BAD_PAGE_LOG)
         csv_link_shown = '%s' % BAD_PAGE_LOG
-        log_table = '''<p><p><p><p><h2><table><tbody>
+        log_table = (
+            '''<p><p><p><p><h2><table><tbody>
             <tr><td>LOG FILES LINK:&nbsp;&nbsp;<td><a href="%s">%s</a></tr>
             <tr><td>RESULTS TABLE:&nbsp;&nbsp;<td><a href="%s">%s</a></tr>
             </tbody></table></h2><p><p><p><p>''' % (
-            web_log_path, log_link_shown, csv_link, csv_link_shown)
+                web_log_path, log_link_shown, csv_link, csv_link_shown
+            )
+        )
 
         failure_table = '<h2><table><tbody></div>'
         any_screenshots = False
         for line in self.page_results_list:
             line = line.split(',')
             if line[1] == '"FAILED!"' or line[1] == '"ERROR!"':
                 if not any_screenshots:
@@ -416,18 +431,17 @@
             if self.check_count == 1:
                 print(warn_msg)
             return
         # This is where the magic happens
         self.manual_page_check(*args)
 
     def auto_close_results(self):
-        ''' If this method is called, the results page will automatically close
+        """If this method is called, the results page will automatically close
         at the end of the test run, rather than waiting on the user to close
-        the results page manually.
-        '''
+        the results page manually."""
         self.auto_close_results_page = True
 
     def tearDown(self):
         if self.headless and self.check_count > 0:
             print("WARNING: %s manual checks were skipped!" % self.check_count)
         if sys.exc_info()[1]:
             self.add_failure(sys.exc_info()[1])
```

### Comparing `masterqa-1.8.3/masterqa/settings.py` & `masterqa-1.8.4/masterqa/settings.py`

 * *Files identical despite different names*

### Comparing `masterqa-1.8.3/masterqa.egg-info/PKG-INFO` & `masterqa-1.8.4/masterqa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterqa
-Version: 1.8.3
+Version: 1.8.4
 Summary: Automation-Assisted Manual Testing - https://masterqa.com
 Home-page: https://github.com/masterqa/MasterQA
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Platform: Windows
```

### Comparing `masterqa-1.8.3/pytest.ini` & `masterqa-1.8.4/pytest.ini`

 * *Files identical despite different names*

### Comparing `masterqa-1.8.3/setup.py` & `masterqa-1.8.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,32 +24,34 @@
     reply = None
     input_method = input
     if not sys.version_info[0] >= 3:
         input_method = raw_input  # noqa
     reply = str(input_method(
         ">>> Confirm release PUBLISH to PyPI? (yes/no): ")).lower().strip()
     if reply == "yes":
+        if sys.version_info < (3, 9):
+            print("\nERROR! Publishing to PyPI requires Python>=3.9")
+            sys.exit()
         print("\n*** Checking code health with flake8:\n")
-        if sys.version_info >= (3, 9):
-            os.system("python -m pip install 'flake8==6.0.0'")
-        else:
-            os.system("python -m pip install 'flake8==5.0.4'")
+        os.system("python -m pip install 'flake8==6.0.0'")
         flake8_status = os.system("flake8 --exclude=recordings,temp")
         if flake8_status != 0:
-            print("\nWARNING! Fix flake8 issues before publishing to PyPI!\n")
+            print("\nERROR! Fix flake8 issues before publishing to PyPI!\n")
             sys.exit()
         else:
             print("*** No flake8 issues detected. Continuing...")
         print("\n*** Removing existing distribution packages: ***\n")
         os.system("rm -f dist/*.egg; rm -f dist/*.tar.gz; rm -f dist/*.whl")
         os.system("rm -rf build/bdist.*; rm -rf build/lib")
         print("\n*** Installing build: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade 'build>=0.10.0'")
         print("\n*** Installing pkginfo: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade 'pkginfo>=1.9.6'")
+        print("\n*** Installing readme-renderer: *** (For PyPI uploads)\n")
+        os.system("python -m pip install --upgrade 'readme-renderer>=40.0'")
         print("\n*** Installing twine: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade 'twine>=4.0.2'")
         print("\n*** Installing tqdm: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade tqdm")
         print("\n*** Rebuilding distribution packages: ***\n")
         os.system("python -m build")  # Create new tar/wheel
         print("\n*** Publishing The Release to PyPI: ***\n")
@@ -57,29 +59,29 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name="masterqa",
-    version="1.8.3",
+    version="1.8.4",
     description="Automation-Assisted Manual Testing - https://masterqa.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     platforms=["Windows", "Linux", "Mac OS-X"],
     url="https://github.com/masterqa/MasterQA",
     author="Michael Mintz",
     author_email="mdmintz@gmail.com",
     maintainer="Michael Mintz",
     license="MIT",
     python_requires=">=3.6",
     install_requires=[
-        "seleniumbase>=4.15.3",
-        "pdbp>=1.4.0",
-        "tabcompleter>=1.2.0",
+        "seleniumbase>=4.15.5",
+        "pdbp>=1.4.1",
+        "tabcompleter>=1.2.1",
         "sbvirtualdisplay>=1.2.0",
     ],
     packages=["masterqa"],
     entry_points={
         "nose.plugins": []
     }
 )
```

