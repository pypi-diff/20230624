# Comparing `tmp/armaqdl-0.9.0.tar.gz` & `tmp/armaqdl-0.9.1.tar.gz`

## Comparing `armaqdl-0.9.0.tar` & `armaqdl-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 armaqdl-0.9.0/.editorconfig
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 armaqdl-0.9.0/.flake8
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 armaqdl-0.9.0/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.9.0/armaqdl/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 armaqdl-0.9.0/armaqdl/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 armaqdl-0.9.0/armaqdl/_version.py
--rw-r--r--   0        0        0    17627 2020-02-02 00:00:00.000000 armaqdl-0.9.0/armaqdl/armaqdl.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 armaqdl-0.9.0/armaqdl/config.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 armaqdl-0.9.0/armaqdl/const.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 armaqdl-0.9.0/armaqdl/update.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 armaqdl-0.9.0/config/settings.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 armaqdl-0.9.0/tests/test_commands.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 armaqdl-0.9.0/tests/test_config.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 armaqdl-0.9.0/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 armaqdl-0.9.0/LICENSE
--rw-r--r--   0        0        0     7347 2020-02-02 00:00:00.000000 armaqdl-0.9.0/README.md
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 armaqdl-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 armaqdl-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 armaqdl-0.9.1/.editorconfig
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 armaqdl-0.9.1/.flake8
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 armaqdl-0.9.1/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.9.1/armaqdl/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 armaqdl-0.9.1/armaqdl/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 armaqdl-0.9.1/armaqdl/_version.py
+-rw-r--r--   0        0        0    17627 2020-02-02 00:00:00.000000 armaqdl-0.9.1/armaqdl/armaqdl.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 armaqdl-0.9.1/armaqdl/config.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 armaqdl-0.9.1/armaqdl/const.py
+-rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 armaqdl-0.9.1/armaqdl/update.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 armaqdl-0.9.1/config/settings.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 armaqdl-0.9.1/tests/test_commands.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 armaqdl-0.9.1/tests/test_config.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 armaqdl-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 armaqdl-0.9.1/LICENSE
+-rw-r--r--   0        0        0     7561 2020-02-02 00:00:00.000000 armaqdl-0.9.1/README.md
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 armaqdl-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 armaqdl-0.9.1/PKG-INFO
```

### Comparing `armaqdl-0.9.0/armaqdl/armaqdl.py` & `armaqdl-0.9.1/armaqdl/armaqdl.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.9.0/armaqdl/config.py` & `armaqdl-0.9.1/armaqdl/config.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.9.0/armaqdl/update.py` & `armaqdl-0.9.1/armaqdl/update.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,49 @@
 import os
 import sys
 import time
 from pathlib import Path
 from urllib import request, error
 
 from ._version import __version_tuple__
-from .const import PACKAGE, CONFIG_DIR, LATEST_FILE
+from .const import PACKAGE, CONFIG_DIR, LATEST_FILE, WINGET_PATH
 
 GITHUB = f"https://github.com/jonpas/{PACKAGE}" + "/releases/download/v{}/armaqdl.exe"
 PYPI = f"https://pypi.org/pypi/{PACKAGE}/json"
 
 
+def get_dist():
+    if is_exe():
+        exe = get_exe()
+        if exe == WINGET_PATH / exe.name:
+            return "winget"
+        return "standalone"
+    return "python"
+
+
+def get_update_info(manager):
+    if manager == "python":
+        return "Update with your Python package manager."
+    if manager == "standalone":
+        return "Run with '--update' to perform a self-update."
+    elif manager == "winget":
+        return "Update with 'winget upgrade armaqdl'."
+    return ""
+
+
 def is_exe():
     return getattr(sys, "frozen", False)
 
 
-def get_exe_old(exe):
+def get_exe():
+    return Path(sys.executable).resolve(strict=True)
+
+
+def get_exe_old():
+    exe = get_exe()
     return exe.parent / f"{exe.stem}_old{exe.suffix}"
 
 
 def is_admin():
     # Linux (no ctypes.windll)
     if os.name == "posix":
         return True
@@ -52,15 +76,15 @@
     current_cmp = __version_tuple__[:3]
 
     return latest_cmp > current_cmp  # True if newer exists
 
 
 def clean():
     if is_exe():
-        old_exe = get_exe_old(Path(sys.executable))
+        old_exe = get_exe_old()
         if old_exe.exists():
             os.remove(old_exe)
 
 
 def check():
     # Check metadata of cached latest version file
     modified = 0
@@ -77,25 +101,23 @@
             print(f"Note: Unable to check for updates. => {e}\n")
             return 1
     else:
         with open(CONFIG_DIR / LATEST_FILE, "r", encoding="utf-8") as f:
             latest = f.read()
 
     if is_newer(latest):
-        if is_exe():
-            print(f"Note: Update v{latest} is available! Run with '--update' to perform a self-update.\n")
-        else:
-            print(f"Note: Update v{latest} is available!\n")
+        print(f"Note: Update v{latest} is available! {get_update_info(get_dist())}\n")
 
     return 0
 
 
 def update():
-    if not is_exe():
-        print("Error! Only standalone executable may be updated!")
+    dist = get_dist()
+    if dist != "standalone":
+        print(f"Error! Only standalone executable may be self-updated! {get_update_info(dist)}")
         return 1
 
     try:
         latest = get_latest()
     except (error.HTTPError, error.URLError) as e:
         print(f"Error! Unable to retrieve latest version! => {e}")
         return 2
@@ -105,19 +127,19 @@
         return 0
 
     if not is_admin():
         # Re-run with admin rights
         print("Administrator permissions required - agree if you would like to continue.")
         ctypes.windll.shell32.ShellExecuteW(None, "runas", sys.executable, " ".join(sys.argv[1:]), None, 1)
 
-    exe = Path(sys.executable)
+    exe = get_exe()
     print(f"Location: {exe}")
 
     # Rename current executable
-    old_exe = get_exe_old(exe)
+    old_exe = get_exe_old()
     os.replace(exe, old_exe)
 
     try:
         request.urlretrieve(GITHUB.format(latest), exe)
     except (error.HTTPError, error.URLError) as e:
         print(f"Error! Unable to download update! => {e}")
         os.replace(old_exe, exe)
```

### Comparing `armaqdl-0.9.0/config/settings.toml` & `armaqdl-0.9.1/config/settings.toml`

 * *Files identical despite different names*

### Comparing `armaqdl-0.9.0/tests/test_commands.py` & `armaqdl-0.9.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.9.0/tests/test_config.py` & `armaqdl-0.9.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.9.0/.gitignore` & `armaqdl-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `armaqdl-0.9.0/LICENSE` & `armaqdl-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `armaqdl-0.9.0/README.md` & `armaqdl-0.9.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # ArmaQDL
 
-[![CI - Test](https://github.com/jonpas/ArmaQDL/actions/workflows/test.yml/badge.svg)](https://github.com/jonpas/ArmaQDL/actions/workflows/test.yml)
-[![CI - Build](https://github.com/jonpas/ArmaQDL/actions/workflows/build.yml/badge.svg)](https://github.com/jonpas/ArmaQDL/actions/workflows/build.yml)
-[![PyPI - Version](https://img.shields.io/pypi/v/ArmaQDL.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/ArmaQDL)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ArmaQDL.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/ArmaQDL)
+[![CI Test](https://github.com/jonpas/ArmaQDL/actions/workflows/test.yml/badge.svg)](https://github.com/jonpas/ArmaQDL/actions/workflows/test.yml)
+[![CI Build](https://github.com/jonpas/ArmaQDL/actions/workflows/build.yml/badge.svg)](https://github.com/jonpas/ArmaQDL/actions/workflows/build.yml)
+[![PyPI](https://img.shields.io/pypi/v/ArmaQDL.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/ArmaQDL)
+[![PyPI Python](https://img.shields.io/pypi/pyversions/ArmaQDL.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/ArmaQDL)
+[![WinGet](https://img.shields.io/badge/WinGet-Run-lightblue.svg)](https://winget.run/pkg/jonpas/ArmaQDL)
 
-Python program for quick launching various mod developement configurations for Arma through a simple CLI.
+Quick launching various mod development configurations for Arma through a simple CLI.
 
 Through easily-identifiable preset locations, this program can provide a fast and developer-friendly CLI with some additional optional features, such as building mods and opening the last log file. It is designed around easily modifiable location groups and build tools.
 
 ## Features
 
 - Easy **mod launching** from different **preset locations**
 - **Load mission** via mission name only or specifying profile name
@@ -22,54 +23,55 @@
 - Load mission on dedicated server (by manipulating `server.cfg`)
 - Join server
 
 
 ## Installation
 
 ArmaQDL is distributed on [PyPI](https://pypi.org/) as well as a Standalone executable (Windows only).
-- Use Standalone if you are on Windows and don't have Python installed.
-- Use PyPI if you have Python installed or are not using Windows.
+- Use [WinGet (recommended)](#winget-(recommended)) or [Standalone](#standalone) if you are on Windows and don't have Python installed.
+- Use [PyPI](#pypi) if you have Python installed or are not using Windows.
 
 PyPI provides easier updating of ArmaQDL, while Standalone requires manual updates.
 
-#### Standalone
-
-Download `armaqdl.exe` from [latest release](https://github.com/jonpas/ArmaQDL/releases/latest) and place it in a convenient location.
+#### WinGet (recommended)
 
-Open Command Prompt, PowerShell or any other terminal application, navigate to the location of `armaqdl.exe` and run it once to generate configuration files without launching Arma.
+Open Command Prompt, PowerShell or any other terminal application and install ArmaQDL.
 
 ```sh
-# Command Prompt
-$ armaqdl
-# PowerShell
-$ .\armaqdl
+$ winget install armaqdl
 ```
-_Note: Add `.exe` if `armaqdl` is not enough to find the executable._
 
+#### Standalone
+
+Download `armaqdl.exe` from [latest release](https://github.com/jonpas/ArmaQDL/releases/latest) and place it in a convenient location.
+
+_Note: Add location directory to `PATH` environmental variable to use it directly._
 
 #### PyPI
 
 Installation as a user is recommended to avoid permission issues with CLI script installation.
 
 ```
 $ pip install --user ArmaQDL
 ```
 _Note: Add pip installation directory to `PATH` environmental variable to use it directly._
 
-Run it once to generate configuration files without launching Arma.
+
+## Setup
+
+Open Command Prompt, PowerShell or any other terminal application, and run ArmaQDL once to generate the configuration files (this will not launch Arma).
 
 ```sh
-# Directly (only works if in PATH)
+# WinGet / CMD / PyPI if in PATH
 $ armaqdl
-# As a Python module
+
+# PyPI as a Python module
 $ python -m armaqdl
 ```
-
-
-## Setup
+_Note: Add `.exe` if `armaqdl` is not enough to find the executable._
 
 You should modify the [default settings](https://github.com/jonpas/ArmaQDL/blob/master/config/settings.toml) to your needs. Launching without setup may create a new profile and result in failed launches.
 
 Settings file can be found in your operating system's standard configuration directory, usually:
 - Windows: `%AppData%\ArmaQDL\settings.toml`
 - Linux: `~/.config/ArmaQDL/settings.toml`
```

### Comparing `armaqdl-0.9.0/pyproject.toml` & `armaqdl-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `armaqdl-0.9.0/PKG-INFO` & `armaqdl-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArmaQDL
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python program for quick launching various mod development configurations for Arma through a simple CLI.
 Project-URL: Homepage, https://github.com/jonpas/Arma-QDL
 Project-URL: Bug Tracker, https://github.com/jonpas/Arma-QDL/issues
 Author-email: Jonpas <jonpas33@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Environment :: Console
@@ -20,20 +20,21 @@
 Requires-Python: >=3.7
 Requires-Dist: platformdirs
 Requires-Dist: toml
 Description-Content-Type: text/markdown
 
 # ArmaQDL
 
-[![CI - Test](https://github.com/jonpas/ArmaQDL/actions/workflows/test.yml/badge.svg)](https://github.com/jonpas/ArmaQDL/actions/workflows/test.yml)
-[![CI - Build](https://github.com/jonpas/ArmaQDL/actions/workflows/build.yml/badge.svg)](https://github.com/jonpas/ArmaQDL/actions/workflows/build.yml)
-[![PyPI - Version](https://img.shields.io/pypi/v/ArmaQDL.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/ArmaQDL)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ArmaQDL.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/ArmaQDL)
+[![CI Test](https://github.com/jonpas/ArmaQDL/actions/workflows/test.yml/badge.svg)](https://github.com/jonpas/ArmaQDL/actions/workflows/test.yml)
+[![CI Build](https://github.com/jonpas/ArmaQDL/actions/workflows/build.yml/badge.svg)](https://github.com/jonpas/ArmaQDL/actions/workflows/build.yml)
+[![PyPI](https://img.shields.io/pypi/v/ArmaQDL.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/ArmaQDL)
+[![PyPI Python](https://img.shields.io/pypi/pyversions/ArmaQDL.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/ArmaQDL)
+[![WinGet](https://img.shields.io/badge/WinGet-Run-lightblue.svg)](https://winget.run/pkg/jonpas/ArmaQDL)
 
-Python program for quick launching various mod developement configurations for Arma through a simple CLI.
+Quick launching various mod development configurations for Arma through a simple CLI.
 
 Through easily-identifiable preset locations, this program can provide a fast and developer-friendly CLI with some additional optional features, such as building mods and opening the last log file. It is designed around easily modifiable location groups and build tools.
 
 ## Features
 
 - Easy **mod launching** from different **preset locations**
 - **Load mission** via mission name only or specifying profile name
@@ -46,54 +47,55 @@
 - Load mission on dedicated server (by manipulating `server.cfg`)
 - Join server
 
 
 ## Installation
 
 ArmaQDL is distributed on [PyPI](https://pypi.org/) as well as a Standalone executable (Windows only).
-- Use Standalone if you are on Windows and don't have Python installed.
-- Use PyPI if you have Python installed or are not using Windows.
+- Use [WinGet (recommended)](#winget-(recommended)) or [Standalone](#standalone) if you are on Windows and don't have Python installed.
+- Use [PyPI](#pypi) if you have Python installed or are not using Windows.
 
 PyPI provides easier updating of ArmaQDL, while Standalone requires manual updates.
 
-#### Standalone
-
-Download `armaqdl.exe` from [latest release](https://github.com/jonpas/ArmaQDL/releases/latest) and place it in a convenient location.
+#### WinGet (recommended)
 
-Open Command Prompt, PowerShell or any other terminal application, navigate to the location of `armaqdl.exe` and run it once to generate configuration files without launching Arma.
+Open Command Prompt, PowerShell or any other terminal application and install ArmaQDL.
 
 ```sh
-# Command Prompt
-$ armaqdl
-# PowerShell
-$ .\armaqdl
+$ winget install armaqdl
 ```
-_Note: Add `.exe` if `armaqdl` is not enough to find the executable._
 
+#### Standalone
+
+Download `armaqdl.exe` from [latest release](https://github.com/jonpas/ArmaQDL/releases/latest) and place it in a convenient location.
+
+_Note: Add location directory to `PATH` environmental variable to use it directly._
 
 #### PyPI
 
 Installation as a user is recommended to avoid permission issues with CLI script installation.
 
 ```
 $ pip install --user ArmaQDL
 ```
 _Note: Add pip installation directory to `PATH` environmental variable to use it directly._
 
-Run it once to generate configuration files without launching Arma.
+
+## Setup
+
+Open Command Prompt, PowerShell or any other terminal application, and run ArmaQDL once to generate the configuration files (this will not launch Arma).
 
 ```sh
-# Directly (only works if in PATH)
+# WinGet / CMD / PyPI if in PATH
 $ armaqdl
-# As a Python module
+
+# PyPI as a Python module
 $ python -m armaqdl
 ```
-
-
-## Setup
+_Note: Add `.exe` if `armaqdl` is not enough to find the executable._
 
 You should modify the [default settings](https://github.com/jonpas/ArmaQDL/blob/master/config/settings.toml) to your needs. Launching without setup may create a new profile and result in failed launches.
 
 Settings file can be found in your operating system's standard configuration directory, usually:
 - Windows: `%AppData%\ArmaQDL\settings.toml`
 - Linux: `~/.config/ArmaQDL/settings.toml`
```

