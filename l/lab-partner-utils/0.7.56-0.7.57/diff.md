# Comparing `tmp/lab-partner-utils-0.7.56.tar.gz` & `tmp/lab-partner-utils-0.7.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab-partner-utils-0.7.56.tar", last modified: Mon Jun 12 02:09:44 2023, max compression
+gzip compressed data, was "lab-partner-utils-0.7.57.tar", last modified: Sat Jun 24 16:18:32 2023, max compression
```

## Comparing `lab-partner-utils-0.7.56.tar` & `lab-partner-utils-0.7.57.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:44.028878 lab-partner-utils-0.7.56/
--rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:44.024878 lab-partner-utils-0.7.56/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:44.024878 lab-partner-utils-0.7.56/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.github/workflows/build-deploy.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3519 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:44.024878 lab-partner-utils-0.7.56/.idea/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.idea/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:44.024878 lab-partner-utils-0.7.56/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.idea/lab-partner-utils.iml
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-06-12 02:09:44.028878 lab-partner-utils-0.7.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (122)      253 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/run.sh
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-12 02:09:44.028878 lab-partner-utils-0.7.56/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:44.024878 lab-partner-utils-0.7.56/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:44.028878 lab-partner-utils-0.7.56/src/lab_partner_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/src/lab_partner_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9043 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/src/lab_partner_utils/cli_command_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1706 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/src/lab_partner_utils/command_builder.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7252 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/src/lab_partner_utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/src/lab_partner_utils/kernel_launcher.py
--rw-r--r--   0 runner    (1001) docker     (122)    13028 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/src/lab_partner_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:44.028878 lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-06-12 02:09:43.000000 lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-12 02:09:44.000000 lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 02:09:43.000000 lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-12 02:09:43.000000 lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-06-12 02:09:43.000000 lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-12 02:09:43.000000 lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/workspace_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-24 16:18:32.453868 lab-partner-utils-0.7.57/
+-rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-24 16:18:32.445868 lab-partner-utils-0.7.57/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-24 16:18:32.449868 lab-partner-utils-0.7.57/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/.github/workflows/build-deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3519 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-24 16:18:32.449868 lab-partner-utils-0.7.57/.idea/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/.idea/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-24 16:18:32.449868 lab-partner-utils-0.7.57/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/.idea/lab-partner-utils.iml
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-06-24 16:18:32.453868 lab-partner-utils-0.7.57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (122)      253 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/run.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-24 16:18:32.453868 lab-partner-utils-0.7.57/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-24 16:18:32.445868 lab-partner-utils-0.7.57/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-24 16:18:32.453868 lab-partner-utils-0.7.57/src/lab_partner_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/src/lab_partner_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9043 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/src/lab_partner_utils/cli_command_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1706 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/src/lab_partner_utils/command_builder.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7252 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/src/lab_partner_utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/src/lab_partner_utils/kernel_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13028 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/src/lab_partner_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-24 16:18:32.453868 lab-partner-utils-0.7.57/src/lab_partner_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-06-24 16:18:32.000000 lab-partner-utils-0.7.57/src/lab_partner_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-24 16:18:32.000000 lab-partner-utils-0.7.57/src/lab_partner_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-24 16:18:32.000000 lab-partner-utils-0.7.57/src/lab_partner_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-24 16:18:32.000000 lab-partner-utils-0.7.57/src/lab_partner_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-06-24 16:18:32.000000 lab-partner-utils-0.7.57/src/lab_partner_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-24 16:18:32.000000 lab-partner-utils-0.7.57/src/lab_partner_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-06-24 16:18:04.000000 lab-partner-utils-0.7.57/workspace_commands.py
```

### Comparing `lab-partner-utils-0.7.56/.gitattributes` & `lab-partner-utils-0.7.57/.gitattributes`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.56/.github/workflows/build-deploy.yml` & `lab-partner-utils-0.7.57/.github/workflows/build-deploy.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.56/.gitignore` & `lab-partner-utils-0.7.57/.gitignore`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.56/LICENSE.md` & `lab-partner-utils-0.7.57/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.56/PKG-INFO` & `lab-partner-utils-0.7.57/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner-utils
-Version: 0.7.56
+Version: 0.7.57
 Summary: Utilities used to embed Lab Partner into python projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-utils-0.7.56/pyproject.toml` & `lab-partner-utils-0.7.57/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     "click==8.1.3",
     "docker==6.0.1",
     "importlib-metadata==6.0.0",
     "astpretty==2.1.0",
     "ipykernel==6.21.2",
     "docstring-parser==0.15",
     "python-dotenv==1.0.0",
-    'tomli >= 1.1.0 ; python_version < "3.11"'
+    'tomli >= 1.1.0 ; python_version < "3.11"',
+    "GitPython==3.1.31"
 ]
 
 [project.optional-dependencies]
 #dev = [""]
 test = ["pytest==7.2.2"]
 
 [project.urls]
```

### Comparing `lab-partner-utils-0.7.56/src/lab_partner_utils/cli_command_factory.py` & `lab-partner-utils-0.7.57/src/lab_partner_utils/cli_command_factory.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.56/src/lab_partner_utils/command_builder.py` & `lab-partner-utils-0.7.57/src/lab_partner_utils/command_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.56/src/lab_partner_utils/commands.py` & `lab-partner-utils-0.7.57/src/lab_partner_utils/commands.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.56/src/lab_partner_utils/kernel_launcher.py` & `lab-partner-utils-0.7.57/src/lab_partner_utils/kernel_launcher.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.56/src/lab_partner_utils/utils.py` & `lab-partner-utils-0.7.57/src/lab_partner_utils/utils.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/PKG-INFO` & `lab-partner-utils-0.7.57/src/lab_partner_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner-utils
-Version: 0.7.56
+Version: 0.7.57
 Summary: Utilities used to embed Lab Partner into python projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/SOURCES.txt` & `lab-partner-utils-0.7.57/src/lab_partner_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

