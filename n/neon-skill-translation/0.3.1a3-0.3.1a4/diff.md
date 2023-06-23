# Comparing `tmp/neon-skill-translation-0.3.1a3.tar.gz` & `tmp/neon-skill-translation-0.3.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-translation-0.3.1a3.tar", last modified: Fri Jun 16 01:01:08 2023, max compression
+gzip compressed data, was "neon-skill-translation-0.3.1a4.tar", last modified: Fri Jun 23 23:01:26 2023, max compression
```

## Comparing `neon-skill-translation-0.3.1a3.tar` & `neon-skill-translation-0.3.1a4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:01:08.847175 neon-skill-translation-0.3.1a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-16 01:01:08.847175 neon-skill-translation-0.3.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:01:08.843175 neon-skill-translation-0.3.1a3/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:01:08.843175 neon-skill-translation-0.3.1a3/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:01:08.843175 neon-skill-translation-0.3.1a3/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/locale/en-us/dialog/language_not_supported.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/locale/en-us/dialog/phrase_in_language.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/locale/en-us/languages.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:01:08.843175 neon-skill-translation-0.3.1a3/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/locale/en-us/vocab/female.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/locale/en-us/vocab/male.voc
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/locale/en-us/vocab/translate_phrase.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:01:08.847175 neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-16 01:01:08.000000 neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-16 01:01:08.000000 neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:01:08.000000 neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-16 01:01:08.000000 neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 01:01:08.000000 neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 01:01:08.000000 neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 01:01:08.847175 neon-skill-translation-0.3.1a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:01:08.847175 neon-skill-translation-0.3.1a3/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:01:08.847175 neon-skill-translation-0.3.1a3/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/ui/Translation.qml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/ui/qmldir
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:01:26.873402 neon-skill-translation-0.3.1a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-23 23:01:22.000000 neon-skill-translation-0.3.1a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-23 23:01:26.873402 neon-skill-translation-0.3.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-23 23:01:22.000000 neon-skill-translation-0.3.1a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-06-23 23:01:22.000000 neon-skill-translation-0.3.1a4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:01:26.869402 neon-skill-translation-0.3.1a4/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:01:26.869402 neon-skill-translation-0.3.1a4/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:01:26.869402 neon-skill-translation-0.3.1a4/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-23 23:01:22.000000 neon-skill-translation-0.3.1a4/locale/en-us/dialog/language_not_supported.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 23:01:22.000000 neon-skill-translation-0.3.1a4/locale/en-us/dialog/phrase_in_language.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-23 23:01:22.000000 neon-skill-translation-0.3.1a4/locale/en-us/languages.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:01:26.869402 neon-skill-translation-0.3.1a4/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 23:01:22.000000 neon-skill-translation-0.3.1a4/locale/en-us/vocab/female.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 23:01:22.000000 neon-skill-translation-0.3.1a4/locale/en-us/vocab/male.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 23:01:22.000000 neon-skill-translation-0.3.1a4/locale/en-us/vocab/translate_phrase.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:01:26.873402 neon-skill-translation-0.3.1a4/neon_skill_translation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-23 23:01:26.000000 neon-skill-translation-0.3.1a4/neon_skill_translation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-23 23:01:26.000000 neon-skill-translation-0.3.1a4/neon_skill_translation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 23:01:26.000000 neon-skill-translation-0.3.1a4/neon_skill_translation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-23 23:01:26.000000 neon-skill-translation-0.3.1a4/neon_skill_translation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-23 23:01:26.000000 neon-skill-translation-0.3.1a4/neon_skill_translation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 23:01:26.000000 neon-skill-translation-0.3.1a4/neon_skill_translation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 23:01:26.873402 neon-skill-translation-0.3.1a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-23 23:01:22.000000 neon-skill-translation-0.3.1a4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-23 23:01:22.000000 neon-skill-translation-0.3.1a4/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:01:26.873402 neon-skill-translation-0.3.1a4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-23 23:01:22.000000 neon-skill-translation-0.3.1a4/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:01:26.873402 neon-skill-translation-0.3.1a4/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-23 23:01:22.000000 neon-skill-translation-0.3.1a4/ui/Translation.qml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 23:01:22.000000 neon-skill-translation-0.3.1a4/ui/qmldir
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-23 23:01:22.000000 neon-skill-translation-0.3.1a4/version.py
```

### Comparing `neon-skill-translation-0.3.1a3/LICENSE.md` & `neon-skill-translation-0.3.1a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-0.3.1a3/PKG-INFO` & `neon-skill-translation-0.3.1a4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: neon-skill-translation
-Version: 0.3.1a3
-Home-page: https://github.com/NeonGeckoCom/skill-translation
-Author: Neongecko
-Author-email: developers@neon.ai
-License: BSD-3-Clause
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # <img src='./logo.svg' card_color="#FF8600" width="50" style="vertical-align:bottom" style="vertical-align:bottom">Translation
 
 ## Summary
 
 Translate phrases between languages.
 
 ## Description
```

### Comparing `neon-skill-translation-0.3.1a3/__init__.py` & `neon-skill-translation-0.3.1a4/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/PKG-INFO` & `neon-skill-translation-0.3.1a4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-translation
-Version: 0.3.1a3
+Version: 0.3.1a4
 Home-page: https://github.com/NeonGeckoCom/skill-translation
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/SOURCES.txt` & `neon-skill-translation-0.3.1a4/neon_skill_translation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-0.3.1a3/setup.py` & `neon-skill-translation-0.3.1a4/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-0.3.1a3/skill.json` & `neon-skill-translation-0.3.1a4/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-0.3.1a3/test/test_skill.py` & `neon-skill-translation-0.3.1a4/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-0.3.1a3/ui/Translation.qml` & `neon-skill-translation-0.3.1a4/ui/Translation.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-0.3.1a3/version.py` & `neon-skill-translation-0.3.1a4/version.py`

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

