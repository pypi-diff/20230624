# Comparing `tmp/churchtoolsapi-0.0.2rc63.post1.tar.gz` & `tmp/churchtoolsapi-0.0.2rc65.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "churchtoolsapi-0.0.2rc63.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "churchtoolsapi-0.0.2rc65.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `churchtoolsapi-0.0.2rc63.post1.tar` & `churchtoolsapi-0.0.2rc65.post1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      340 2023-06-22 01:00:36.997812 churchtoolsapi-0.0.2rc63.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1252 2023-06-22 01:00:36.997812 churchtoolsapi-0.0.2rc63.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0       10 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/.github/CODEOWNERS
--rw-r--r--   0        0        0      417 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      245 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/.github/issue-branch.yml
--rw-r--r--   0        0        0      418 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/.github/template-sync.yml
--rw-r--r--   0        0        0     1501 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      671 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      368 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      303 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/.gitignore
--rw-r--r--   0        0        0     1540 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/.pypirc
--rw-r--r--   0        0        0      458 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/.vscode/launch.json
--rw-r--r--   0        0        0      875 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/.vscode/settings.json
--rw-r--r--   0        0        0      444 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1146 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/LICENSE
--rw-r--r--   0        0        0    15868 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/README.md
--rw-r--r--   0        0        0     2780 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/SECURITY.md
--rw-r--r--   0        0        0     1308 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/SUPPORT.md
--rw-r--r--   0        0        0      634 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/docs/Makefile
--rw-r--r--   0        0        0     2356 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/docs/conf.py
--rw-r--r--   0        0        0      359 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/docs/developer.md
--rw-r--r--   0        0        0      468 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/docs/index.rst
--rw-r--r--   0        0        0      800 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/docs/make.bat
--rw-r--r--   0        0        0       57 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/docs/modules.rst
--rw-r--r--   0        0        0      471 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16089 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/docs/pyproject.md
--rw-r--r--   0        0        0      437 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      427 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/docs/python_package.rst
--rw-r--r--   0        0        0       42 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/docs/requirements.txt
--rw-r--r--   0        0        0       44 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/docs/vscode.md
--rw-r--r--   0        0        0      208 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/docs/workflows.md
--rw-r--r--   0        0        0     6885 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/pyproject.toml
--rw-r--r--   0        0        0      396 2023-06-22 01:00:51.930040 churchtoolsapi-0.0.2rc63.post1/src/ChurchToolsApi/__init__.py
--rw-r--r--   0        0        0     5005 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/src/ChurchToolsApi/churchtools_api.py
--rw-r--r--   0        0        0     1307 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/src/ChurchToolsApi/exceptions.py
--rw-r--r--   0        0        0       43 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/src/README.md
--rw-r--r--   0        0        0     2445 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/tests/conftest.py
--rw-r--r--   0        0        0     2595 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/tests/test_churchtools_api.py
--rw-r--r--   0        0        0      745 2023-06-22 01:00:37.001813 churchtoolsapi-0.0.2rc63.post1/tests/test_integrations.py
--rw-r--r--   0        0        0    17799 1970-01-01 00:00:00.000000 churchtoolsapi-0.0.2rc63.post1/PKG-INFO
+-rw-r--r--   0        0        0      340 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1252 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0       10 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      417 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      245 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.github/issue-branch.yml
+-rw-r--r--   0        0        0      418 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.github/template-sync.yml
+-rw-r--r--   0        0        0     1501 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      671 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      318 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      368 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      303 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.pypirc
+-rw-r--r--   0        0        0      458 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.vscode/launch.json
+-rw-r--r--   0        0        0      875 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/.vscode/settings.json
+-rw-r--r--   0        0        0      444 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1146 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/LICENSE
+-rw-r--r--   0        0        0    15868 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/README.md
+-rw-r--r--   0        0        0     2780 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/SECURITY.md
+-rw-r--r--   0        0        0     1308 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/SUPPORT.md
+-rw-r--r--   0        0        0      634 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/docs/Makefile
+-rw-r--r--   0        0        0     2356 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/docs/conf.py
+-rw-r--r--   0        0        0      359 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/docs/developer.md
+-rw-r--r--   0        0        0      468 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/docs/make.bat
+-rw-r--r--   0        0        0       57 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16089 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      437 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      427 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2023-06-24 01:40:12.700119 churchtoolsapi-0.0.2rc65.post1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2023-06-24 01:40:12.704119 churchtoolsapi-0.0.2rc65.post1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2023-06-24 01:40:12.704119 churchtoolsapi-0.0.2rc65.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6885 2023-06-24 01:40:12.704119 churchtoolsapi-0.0.2rc65.post1/pyproject.toml
+-rw-r--r--   0        0        0      396 2023-06-24 01:40:27.664352 churchtoolsapi-0.0.2rc65.post1/src/ChurchToolsApi/__init__.py
+-rw-r--r--   0        0        0     5005 2023-06-24 01:40:12.704119 churchtoolsapi-0.0.2rc65.post1/src/ChurchToolsApi/churchtools_api.py
+-rw-r--r--   0        0        0     1307 2023-06-24 01:40:12.704119 churchtoolsapi-0.0.2rc65.post1/src/ChurchToolsApi/exceptions.py
+-rw-r--r--   0        0        0       43 2023-06-24 01:40:12.704119 churchtoolsapi-0.0.2rc65.post1/src/README.md
+-rw-r--r--   0        0        0     2445 2023-06-24 01:40:12.704119 churchtoolsapi-0.0.2rc65.post1/tests/conftest.py
+-rw-r--r--   0        0        0     2595 2023-06-24 01:40:12.704119 churchtoolsapi-0.0.2rc65.post1/tests/test_churchtools_api.py
+-rw-r--r--   0        0        0      745 2023-06-24 01:40:12.704119 churchtoolsapi-0.0.2rc65.post1/tests/test_integrations.py
+-rw-r--r--   0        0        0    17799 1970-01-01 00:00:00.000000 churchtoolsapi-0.0.2rc65.post1/PKG-INFO
```

### Comparing `churchtoolsapi-0.0.2rc63.post1/.devcontainer/devcontainer.json` & `churchtoolsapi-0.0.2rc65.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/.github/workflows/CI.yml` & `churchtoolsapi-0.0.2rc65.post1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/.github/workflows/schedule-update-actions.yml` & `churchtoolsapi-0.0.2rc65.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/.gitignore` & `churchtoolsapi-0.0.2rc65.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/.pre-commit-config.yaml` & `churchtoolsapi-0.0.2rc65.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/.vscode/settings.json` & `churchtoolsapi-0.0.2rc65.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/LICENSE` & `churchtoolsapi-0.0.2rc65.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/README.md` & `churchtoolsapi-0.0.2rc65.post1/README.md`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/SECURITY.md` & `churchtoolsapi-0.0.2rc65.post1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/SUPPORT.md` & `churchtoolsapi-0.0.2rc65.post1/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/docs/Makefile` & `churchtoolsapi-0.0.2rc65.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/docs/conf.py` & `churchtoolsapi-0.0.2rc65.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/docs/make.bat` & `churchtoolsapi-0.0.2rc65.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/docs/pylint.md` & `churchtoolsapi-0.0.2rc65.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/pyproject.toml` & `churchtoolsapi-0.0.2rc65.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "flake8-pyproject",
     "pre-commit==3.3.3",
     "pylint==2.17.4",
     "pylint_junit",
     "pytest-cov==4.1.0",
     "pytest-mock<3.11.2",
     "pytest-runner",
-    "pytest==7.3.2",
+    "pytest==7.4.0",
     "pytest-github-actions-annotate-failures",
     "shellcheck-py==0.9.0.5",
     "responses==0.23.1",
 ]
 
 [project.urls]
 Documentation = "https://github.com/microsoft/python-package-template/tree/main#readme"
```

### Comparing `churchtoolsapi-0.0.2rc63.post1/src/ChurchToolsApi/churchtools_api.py` & `churchtoolsapi-0.0.2rc65.post1/src/ChurchToolsApi/churchtools_api.py`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/src/ChurchToolsApi/exceptions.py` & `churchtoolsapi-0.0.2rc65.post1/src/ChurchToolsApi/exceptions.py`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/tests/conftest.py` & `churchtoolsapi-0.0.2rc65.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/tests/test_churchtools_api.py` & `churchtoolsapi-0.0.2rc65.post1/tests/test_churchtools_api.py`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/tests/test_integrations.py` & `churchtoolsapi-0.0.2rc65.post1/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `churchtoolsapi-0.0.2rc63.post1/PKG-INFO` & `churchtoolsapi-0.0.2rc65.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChurchToolsApi
-Version: 0.0.2rc63.post1
+Version: 0.0.2rc65.post1
 Summary: A Python wrapper for the ChurchTools API
 Author-email: Felix Kotschenreuther <felix.kotschenreuther@gmail.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -24,15 +24,15 @@
 Requires-Dist: flake8-pyproject ; extra == "test"
 Requires-Dist: pre-commit==3.3.3 ; extra == "test"
 Requires-Dist: pylint==2.17.4 ; extra == "test"
 Requires-Dist: pylint_junit ; extra == "test"
 Requires-Dist: pytest-cov==4.1.0 ; extra == "test"
 Requires-Dist: pytest-mock<3.11.2 ; extra == "test"
 Requires-Dist: pytest-runner ; extra == "test"
-Requires-Dist: pytest==7.3.2 ; extra == "test"
+Requires-Dist: pytest==7.4.0 ; extra == "test"
 Requires-Dist: pytest-github-actions-annotate-failures ; extra == "test"
 Requires-Dist: shellcheck-py==0.9.0.5 ; extra == "test"
 Requires-Dist: responses==0.23.1 ; extra == "test"
 Project-URL: Documentation, https://github.com/microsoft/python-package-template/tree/main#readme
 Project-URL: Source, https://github.com/microsoft/python-package-template
 Project-URL: Tracker, https://github.com/microsoft/python-package-template/issues
 Provides-Extra: spark
```

