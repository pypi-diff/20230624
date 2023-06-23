# Comparing `tmp/neon-skill-demo-0.3.1a3.tar.gz` & `tmp/neon-skill-demo-0.3.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-demo-0.3.1a3.tar", last modified: Thu Jun 15 20:51:54 2023, max compression
+gzip compressed data, was "neon-skill-demo-0.3.1a4.tar", last modified: Fri Jun 23 23:32:29 2023, max compression
```

## Comparing `neon-skill-demo-0.3.1a3.tar` & `neon-skill-demo-0.3.1a4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:51:54.573998 neon-skill-demo-0.3.1a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-15 20:51:54.573998 neon-skill-demo-0.3.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:51:54.569998 neon-skill-demo-0.3.1a3/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:51:54.569998 neon-skill-demo-0.3.1a3/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/en-us/ask_demo.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/en-us/ask_demo_next_time.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/en-us/confirm_demo_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/en-us/confirm_demo_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/en-us/demo.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/en-us/finished_demo.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/en-us/mall_demo.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/en-us/show_demo.intent
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/en-us/starting_demo.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:51:54.573998 neon-skill-demo-0.3.1a3/locale/uk-ua/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/uk-ua/ask_demo.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/uk-ua/ask_demo_next_time.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/uk-ua/confirm_demo_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/uk-ua/confirm_demo_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/uk-ua/demo.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/uk-ua/finished_demo.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/uk-ua/show_demo.intent
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/locale/uk-ua/starting_demo.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:51:54.573998 neon-skill-demo-0.3.1a3/neon_skill_demo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-15 20:51:54.000000 neon-skill-demo-0.3.1a3/neon_skill_demo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-15 20:51:54.000000 neon-skill-demo-0.3.1a3/neon_skill_demo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:51:54.000000 neon-skill-demo-0.3.1a3/neon_skill_demo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 20:51:54.000000 neon-skill-demo-0.3.1a3/neon_skill_demo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 20:51:54.000000 neon-skill-demo-0.3.1a3/neon_skill_demo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 20:51:54.000000 neon-skill-demo-0.3.1a3/neon_skill_demo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:51:54.573998 neon-skill-demo-0.3.1a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:51:54.573998 neon-skill-demo-0.3.1a3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 20:51:50.000000 neon-skill-demo-0.3.1a3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:32:29.887760 neon-skill-demo-0.3.1a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-23 23:32:29.887760 neon-skill-demo-0.3.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:32:29.883760 neon-skill-demo-0.3.1a4/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:32:29.883760 neon-skill-demo-0.3.1a4/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/en-us/ask_demo.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/en-us/ask_demo_next_time.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/en-us/confirm_demo_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/en-us/confirm_demo_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/en-us/demo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/en-us/finished_demo.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/en-us/mall_demo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/en-us/show_demo.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/en-us/starting_demo.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:32:29.883760 neon-skill-demo-0.3.1a4/locale/uk-ua/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/uk-ua/ask_demo.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/uk-ua/ask_demo_next_time.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/uk-ua/confirm_demo_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/uk-ua/confirm_demo_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/uk-ua/demo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/uk-ua/finished_demo.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/uk-ua/show_demo.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/locale/uk-ua/starting_demo.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:32:29.887760 neon-skill-demo-0.3.1a4/neon_skill_demo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-23 23:32:29.000000 neon-skill-demo-0.3.1a4/neon_skill_demo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-23 23:32:29.000000 neon-skill-demo-0.3.1a4/neon_skill_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 23:32:29.000000 neon-skill-demo-0.3.1a4/neon_skill_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 23:32:29.000000 neon-skill-demo-0.3.1a4/neon_skill_demo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-23 23:32:29.000000 neon-skill-demo-0.3.1a4/neon_skill_demo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 23:32:29.000000 neon-skill-demo-0.3.1a4/neon_skill_demo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 23:32:29.887760 neon-skill-demo-0.3.1a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:32:29.887760 neon-skill-demo-0.3.1a4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-23 23:32:26.000000 neon-skill-demo-0.3.1a4/version.py
```

### Comparing `neon-skill-demo-0.3.1a3/LICENSE.md` & `neon-skill-demo-0.3.1a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-demo-0.3.1a3/PKG-INFO` & `neon-skill-demo-0.3.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-demo
-Version: 0.3.1a3
+Version: 0.3.1a4
 Home-page: https://github.com/NeonGeckoCom/skill-demo
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-demo-0.3.1a3/README.md` & `neon-skill-demo-0.3.1a4/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-demo-0.3.1a3/__init__.py` & `neon-skill-demo-0.3.1a4/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 from mycroft.skills import intent_file_handler
 from mycroft.skills.skill_data import find_resource
 
 
 class DemoSkill(NeonSkill):
     def __init__(self, **kwargs):
-        super(DemoSkill, self).__init__(**kwargs)
+        NeonSkill.__init__(self, **kwargs)
         self._active_demos = dict()
         self._audio_output_done = Event()
         self._prompt_handled = Event()
         self._last_response = None
         self._data_path = get_xdg_data_save_path()
 
     @classproperty
```

### Comparing `neon-skill-demo-0.3.1a3/neon_skill_demo.egg-info/PKG-INFO` & `neon-skill-demo-0.3.1a4/neon_skill_demo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-demo
-Version: 0.3.1a3
+Version: 0.3.1a4
 Home-page: https://github.com/NeonGeckoCom/skill-demo
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-demo-0.3.1a3/neon_skill_demo.egg-info/SOURCES.txt` & `neon-skill-demo-0.3.1a4/neon_skill_demo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-demo-0.3.1a3/setup.py` & `neon-skill-demo-0.3.1a4/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-demo-0.3.1a3/skill.json` & `neon-skill-demo-0.3.1a4/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-demo-0.3.1a3/test/test_skill.py` & `neon-skill-demo-0.3.1a4/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-demo-0.3.1a3/version.py` & `neon-skill-demo-0.3.1a4/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.3.1a3"
+__version__ = "0.3.1a4"
```

