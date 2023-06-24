# Comparing `tmp/pytest_time-0.2.0.tar.gz` & `tmp/pytest_time-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_time-0.2.0.tar", last modified: Fri Jun 16 22:36:36 2023, max compression
+gzip compressed data, was "pytest_time-0.3.0.tar", last modified: Sat Jun 24 18:16:09 2023, max compression
```

## Comparing `pytest_time-0.2.0.tar` & `pytest_time-0.3.0.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 22:36:36.291023 pytest_time-0.2.0/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      723 2023-03-01 18:11:13.000000 pytest_time-0.2.0/.editorconfig
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 22:36:36.287023 pytest_time-0.2.0/.github/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      179 2023-03-01 18:11:13.000000 pytest_time-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      362 2023-06-15 05:03:00.000000 pytest_time-0.2.0/.github/release-drafter.yml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3504 2023-05-22 16:14:08.000000 pytest_time-0.2.0/.github/renovate.json5
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 22:36:36.287023 pytest_time-0.2.0/.github/workflows/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      347 2023-06-08 02:02:37.000000 pytest_time-0.2.0/.github/workflows/release-drafter.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2500 2023-06-11 20:35:38.000000 pytest_time-0.2.0/.github/workflows/tests.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4827 2023-06-15 04:05:36.000000 pytest_time-0.2.0/.gitignore
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      921 2023-05-22 16:14:08.000000 pytest_time-0.2.0/.pre-commit-config.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     7652 2023-06-15 05:04:51.000000 pytest_time-0.2.0/COPYING
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1017 2023-06-16 22:36:36.291023 pytest_time-0.2.0/PKG-INFO
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      153 2023-06-15 00:24:20.000000 pytest_time-0.2.0/README.rst
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     6729 2023-06-16 22:26:12.000000 pytest_time-0.2.0/pyproject.toml
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 22:36:36.287023 pytest_time-0.2.0/pytester/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       31 2023-06-15 04:59:41.000000 pytest_time-0.2.0/pytester/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1091 2023-06-15 04:59:15.000000 pytest_time-0.2.0/pytester/test_instant_sleep.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       38 2023-06-16 22:36:36.291023 pytest_time-0.2.0/setup.cfg
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 22:36:36.287023 pytest_time-0.2.0/src/
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 22:36:36.287023 pytest_time-0.2.0/src/pytest_time/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      450 2023-06-16 22:36:03.000000 pytest_time-0.2.0/src/pytest_time/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      160 2023-06-16 22:36:36.000000 pytest_time-0.2.0/src/pytest_time/_version.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1897 2023-06-15 04:52:37.000000 pytest_time-0.2.0/src/pytest_time/fake_time.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1191 2023-06-16 21:52:50.000000 pytest_time-0.2.0/src/pytest_time/instant_sleep.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1017 2023-06-16 22:22:53.000000 pytest_time-0.2.0/src/pytest_time/mock_time.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2023-06-15 03:51:25.000000 pytest_time-0.2.0/src/pytest_time/py.typed
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      221 2023-06-15 04:06:50.000000 pytest_time-0.2.0/src/pytest_time/real_time.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 22:36:36.291023 pytest_time-0.2.0/src/pytest_time.egg-info/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1017 2023-06-16 22:36:36.000000 pytest_time-0.2.0/src/pytest_time.egg-info/PKG-INFO
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      951 2023-06-16 22:36:36.000000 pytest_time-0.2.0/src/pytest_time.egg-info/SOURCES.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        1 2023-06-16 22:36:36.000000 pytest_time-0.2.0/src/pytest_time.egg-info/dependency_links.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       37 2023-06-16 22:36:36.000000 pytest_time-0.2.0/src/pytest_time.egg-info/entry_points.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      254 2023-06-16 22:36:36.000000 pytest_time-0.2.0/src/pytest_time.egg-info/requires.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       12 2023-06-16 22:36:36.000000 pytest_time-0.2.0/src/pytest_time.egg-info/top_level.txt
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 22:36:36.291023 pytest_time-0.2.0/tests/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2023-06-15 02:52:45.000000 pytest_time-0.2.0/tests/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       30 2023-06-15 04:52:37.000000 pytest_time-0.2.0/tests/conftest.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 22:36:36.291023 pytest_time-0.2.0/tests/integration/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2023-06-15 04:17:24.000000 pytest_time-0.2.0/tests/integration/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      227 2023-06-15 04:52:37.000000 pytest_time-0.2.0/tests/integration/test_instant_sleep.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 22:36:36.291023 pytest_time-0.2.0/tests/unit/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2023-06-15 04:07:43.000000 pytest_time-0.2.0/tests/unit/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1517 2023-06-15 04:46:29.000000 pytest_time-0.2.0/tests/unit/test_fake_time.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1936 2023-06-16 22:34:48.000000 pytest_time-0.2.0/tests/unit/test_instant_sleep.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      911 2023-06-16 22:32:34.000000 pytest_time-0.2.0/tests/unit/test_mock_time.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4714 2023-06-15 05:03:00.000000 pytest_time-0.2.0/tox.ini
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-24 18:16:09.791841 pytest_time-0.3.0/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      723 2023-03-01 18:11:13.000000 pytest_time-0.3.0/.editorconfig
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-24 18:16:09.787841 pytest_time-0.3.0/.github/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      179 2023-03-01 18:11:13.000000 pytest_time-0.3.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      362 2023-06-15 05:03:00.000000 pytest_time-0.3.0/.github/release-drafter.yml
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     3504 2023-05-22 16:14:08.000000 pytest_time-0.3.0/.github/renovate.json5
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-24 18:16:09.787841 pytest_time-0.3.0/.github/workflows/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      347 2023-06-08 02:02:37.000000 pytest_time-0.3.0/.github/workflows/release-drafter.yaml
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     2500 2023-06-11 20:35:38.000000 pytest_time-0.3.0/.github/workflows/tests.yaml
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     4827 2023-06-15 04:05:36.000000 pytest_time-0.3.0/.gitignore
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      921 2023-05-22 16:14:08.000000 pytest_time-0.3.0/.pre-commit-config.yaml
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      188 2023-03-01 18:11:13.000000 pytest_time-0.3.0/.yamllint.yaml
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     7652 2023-06-15 05:04:51.000000 pytest_time-0.3.0/COPYING
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     5116 2023-06-24 18:16:09.791841 pytest_time-0.3.0/PKG-INFO
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     4252 2023-06-24 18:13:42.000000 pytest_time-0.3.0/README.rst
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     6718 2023-06-24 18:05:43.000000 pytest_time-0.3.0/pyproject.toml
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-24 18:16:09.787841 pytest_time-0.3.0/pytester/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)       31 2023-06-15 04:59:41.000000 pytest_time-0.3.0/pytester/__init__.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     1439 2023-06-24 18:03:38.000000 pytest_time-0.3.0/pytester/test_instant_sleep.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      486 2023-06-24 18:01:39.000000 pytest_time-0.3.0/pytester/test_mock_instant_sleep.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      460 2023-06-24 18:01:39.000000 pytest_time-0.3.0/pytester/test_mock_time.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)       38 2023-06-24 18:16:09.791841 pytest_time-0.3.0/setup.cfg
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-24 18:16:09.783841 pytest_time-0.3.0/src/
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-24 18:16:09.787841 pytest_time-0.3.0/src/pytest_time/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     1049 2023-06-24 18:09:13.000000 pytest_time-0.3.0/src/pytest_time/__init__.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      160 2023-06-24 18:16:09.000000 pytest_time-0.3.0/src/pytest_time/_version.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     1897 2023-06-15 04:52:37.000000 pytest_time-0.3.0/src/pytest_time/fake_time.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     1191 2023-06-16 21:52:50.000000 pytest_time-0.3.0/src/pytest_time/instant_sleep.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2023-06-15 03:51:25.000000 pytest_time-0.3.0/src/pytest_time/py.typed
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      221 2023-06-15 04:06:50.000000 pytest_time-0.3.0/src/pytest_time/real_time.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     1082 2023-06-24 18:08:41.000000 pytest_time-0.3.0/src/pytest_time/wrap_time.py
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-24 18:16:09.787841 pytest_time-0.3.0/src/pytest_time.egg-info/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     5116 2023-06-24 18:16:09.000000 pytest_time-0.3.0/src/pytest_time.egg-info/PKG-INFO
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     1029 2023-06-24 18:16:09.000000 pytest_time-0.3.0/src/pytest_time.egg-info/SOURCES.txt
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)        1 2023-06-24 18:16:09.000000 pytest_time-0.3.0/src/pytest_time.egg-info/dependency_links.txt
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)       37 2023-06-24 18:16:09.000000 pytest_time-0.3.0/src/pytest_time.egg-info/entry_points.txt
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      286 2023-06-24 18:16:09.000000 pytest_time-0.3.0/src/pytest_time.egg-info/requires.txt
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)       12 2023-06-24 18:16:09.000000 pytest_time-0.3.0/src/pytest_time.egg-info/top_level.txt
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-24 18:16:09.787841 pytest_time-0.3.0/tests/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)       28 2023-06-24 18:06:18.000000 pytest_time-0.3.0/tests/__init__.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)       64 2023-06-24 18:06:18.000000 pytest_time-0.3.0/tests/conftest.py
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-24 18:16:09.787841 pytest_time-0.3.0/tests/integration/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)       25 2023-06-24 18:06:34.000000 pytest_time-0.3.0/tests/integration/__init__.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      601 2023-06-24 18:04:55.000000 pytest_time-0.3.0/tests/integration/test_with_pytester.py
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-24 18:16:09.791841 pytest_time-0.3.0/tests/unit/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)       18 2023-06-24 18:06:34.000000 pytest_time-0.3.0/tests/unit/__init__.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     1526 2023-06-24 18:04:55.000000 pytest_time-0.3.0/tests/unit/test_fake_time.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     1936 2023-06-16 22:34:48.000000 pytest_time-0.3.0/tests/unit/test_instant_sleep.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      911 2023-06-24 18:01:39.000000 pytest_time-0.3.0/tests/unit/test_mock_time.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     4806 2023-06-24 17:07:21.000000 pytest_time-0.3.0/tox.ini
```

### Comparing `pytest_time-0.2.0/.editorconfig` & `pytest_time-0.3.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `pytest_time-0.2.0/.github/renovate.json5` & `pytest_time-0.3.0/.github/renovate.json5`

 * *Files identical despite different names*

### Comparing `pytest_time-0.2.0/.github/workflows/tests.yaml` & `pytest_time-0.3.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pytest_time-0.2.0/.gitignore` & `pytest_time-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_time-0.2.0/.pre-commit-config.yaml` & `pytest_time-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest_time-0.2.0/COPYING` & `pytest_time-0.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `pytest_time-0.2.0/pyproject.toml` & `pytest_time-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     "pytest-check",
     "pytest-cov==4.1.0",
     "pytest-mock==3.10.0",
 ]
 lint = [
     "black>=23.3.0,<24",
     "codespell[toml]>=2.2.4,<3",
-    "ruff==0.0.269",
+    "rstcheck[sphinx,toml]>=6.0.0,<7",
+    "ruff==0.0.275",
     "yamllint>=1.32.0,<2"
 ]
 types = [
     "mypy[reports]>=1.3.0,<2",
     "pyright==1.1.311",
 ]
 
@@ -170,28 +171,28 @@
     "RUF001", "RUF002", "RUF003",  # Ambiguous unicode characters
     "RUF005",  # Encourages unpacking rather than concatenation
     "RUF008",  # Do not use mutable default values for dataclass attributes
     "RUF100",  # #noqa directive that doesn't flag anything
 ]
 ignore = [
     "ANN10",  # Type annotations for `self` and `cls`
-    #"E203",  # Whitespace before ":"  -- Commented because ruff doesn't currently check E203
     "E501",  # Line too long (reason: black will automatically fix this for us)
     "D105",  # Missing docstring in magic method (reason: magic methods already have definitions)
     "D107",  # Missing docstring in __init__ (reason: documented in class docstring)
     "D203",  # 1 blank line required before class docstring (reason: pep257 default)
     "D213",  # Multi-line docstring summary should start at the second line (reason: pep257 default)
     "D215",  # Section underline is over-indented (reason: pep257 default)
     "A003",  # Class attribute shadowing built-in (reason: Class attributes don't often get bare references)
 ]
 
 [tool.ruff.per-file-ignores]
-"tests/**.py" = [  # Some things we want for the moin project are unnecessary in tests.
+"test_*.py" = [  # Some things we want for the moin project are unnecessary in tests.
     "D",  # Ignore docstring rules in tests
     "ANN", # Ignore type annotations in tests
     "S101",  # Allow assertions in tests
     "S103", # Allow `os.chmod` setting a permissive mask `0o555` on file or directory
     "S108", # Allow Probable insecure usage of temporary file or directory
     "PLR0913",  # Allow many arguments for test functions
+    "PLR2004",  # Allow magic values in tests
 ]
 # isort leaves init files alone by default, this makes ruff ignore them too.
 "__init__.py" = ["I001"]
```

### Comparing `pytest_time-0.2.0/pytester/test_instant_sleep.py` & `pytest_time-0.3.0/pytester/test_instant_sleep.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,7 +34,19 @@
 @pytest.mark.usefixtures("instant_sleep")
 @pytest.mark.parametrize("ms", [0, 1, 10, 100, 1000, 1_000_000])
 def test_snooze_with_mock_sleep(ms: int, mock_sleep: mock.Mock) -> None:
     """Tests that snooze works even when I mock out sleep."""
     snooze(ms)
 
     mock_sleep.assert_called_once_with(ms * 0.001)
+
+
+@pytest.mark.parametrize("sleep_time", [1, 10, 100])
+@pytest.mark.usefixtures("instant_sleep")
+def test_instant_sleep(sleep_time) -> None:
+    start_time = time.time()
+    start_monotonic = time.monotonic()
+
+    time.sleep(sleep_time)
+
+    assert time.time() >= start_time + sleep_time
+    assert time.monotonic() >= start_monotonic + sleep_time
```

### Comparing `pytest_time-0.2.0/src/pytest_time/fake_time.py` & `pytest_time-0.3.0/src/pytest_time/fake_time.py`

 * *Files identical despite different names*

### Comparing `pytest_time-0.2.0/src/pytest_time/instant_sleep.py` & `pytest_time-0.3.0/src/pytest_time/instant_sleep.py`

 * *Files identical despite different names*

### Comparing `pytest_time-0.2.0/src/pytest_time/mock_time.py` & `pytest_time-0.3.0/src/pytest_time/wrap_time.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """A pytest fixture for mocking time calls to record them."""
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
 from unittest import mock
 
-import pytest
+if TYPE_CHECKING:
+    import pytest
 
-from pytest_time import fake_time
+    from pytest_time import fake_time
 
 
-class MockWrapper():
+class MockWrapper:
     """Wraps a time faker with mocks."""
 
-    def __init__(self, faker: fake_time.FakeTime):
+    def __init__(self, faker: fake_time.FakeTime) -> None:
         super().__init__()
         self.sleep = mock.Mock(wraps=faker.sleep)
         self.time = mock.Mock(wraps=faker.time)
         self.time_ns = mock.Mock(wraps=faker.time_ns)
         self.monotonic = mock.Mock(wraps=faker.monotonic)
         self.monotonic_ns = mock.Mock(wraps=faker.monotonic_ns)
```

### Comparing `pytest_time-0.2.0/src/pytest_time.egg-info/SOURCES.txt` & `pytest_time-0.3.0/src/pytest_time.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 .editorconfig
 .gitignore
 .pre-commit-config.yaml
+.yamllint.yaml
 COPYING
 README.rst
 pyproject.toml
 tox.ini
 .github/PULL_REQUEST_TEMPLATE.md
 .github/release-drafter.yml
 .github/renovate.json5
 .github/workflows/release-drafter.yaml
 .github/workflows/tests.yaml
 pytester/__init__.py
 pytester/test_instant_sleep.py
+pytester/test_mock_instant_sleep.py
+pytester/test_mock_time.py
 src/pytest_time/__init__.py
 src/pytest_time/_version.py
 src/pytest_time/fake_time.py
 src/pytest_time/instant_sleep.py
-src/pytest_time/mock_time.py
 src/pytest_time/py.typed
 src/pytest_time/real_time.py
+src/pytest_time/wrap_time.py
 src/pytest_time.egg-info/PKG-INFO
 src/pytest_time.egg-info/SOURCES.txt
 src/pytest_time.egg-info/dependency_links.txt
 src/pytest_time.egg-info/entry_points.txt
 src/pytest_time.egg-info/requires.txt
 src/pytest_time.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/integration/__init__.py
-tests/integration/test_instant_sleep.py
+tests/integration/test_with_pytester.py
 tests/unit/__init__.py
 tests/unit/test_fake_time.py
 tests/unit/test_instant_sleep.py
 tests/unit/test_mock_time.py
```

### Comparing `pytest_time-0.2.0/tests/unit/test_fake_time.py` & `pytest_time-0.3.0/tests/unit/test_fake_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,17 @@
     new = getattr(fft, fn)
     pytest_check.not_equal(original, new)
     pytest_check.equal(patched, new)
     pytest_check.not_equal(patched, original)
 
 
 class FakeFakeTime(fake_time.FakeTime):
-    """A fake class for testing FakeTime"""
+    """A fake class for testing FakeTime."""
 
-    def __init__(self, now: int = 0):
+    def __init__(self, now: int = 0) -> None:
         super().__init__()
         self.now = now
 
     def time_ns(self) -> int:
         return self.now
 
     def monotonic_ns(self) -> int:
```

### Comparing `pytest_time-0.2.0/tests/unit/test_instant_sleep.py` & `pytest_time-0.3.0/tests/unit/test_instant_sleep.py`

 * *Files identical despite different names*

### Comparing `pytest_time-0.2.0/tests/unit/test_mock_time.py` & `pytest_time-0.3.0/tests/unit/test_mock_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Tests for the MockWrapper."""
 import time
 from unittest import mock
 
 import pytest
 import pytest_check
 
-from pytest_time import fake_time, mock_time, real_time
+from pytest_time import fake_time, real_time, wrap_time
 
 
 @pytest.fixture()
 def mock_wrapper():
     mock_faker = mock.Mock(spec=fake_time.FakeTime)
-    return mock_time.MockWrapper(mock_faker)
+    return wrap_time.MockWrapper(mock_faker)
 
 
 def test_install(monkeypatch, mock_wrapper):
     def check_monkeypatch(fn: str, cls):
         patched = getattr(time, fn)
         original = getattr(real_time, fn)
         new = getattr(cls, fn)
```

### Comparing `pytest_time-0.2.0/tox.ini` & `pytest_time-0.3.0/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -54,70 +54,71 @@
 env_dir = {work_dir}/linting
 runner = ignore_env_name_mismatch
 
 [shellcheck]
 find = git ls-files
 filter = file --mime-type -Nnf- | grep shellscript | cut -f1 -d:
 
-[testenv:lint-{black,ruff,shellcheck,codespell,yaml}]
+[testenv:lint-{black,codespell,rst,ruff,shellcheck,yaml}]
 description = Lint the source code
 base = testenv, lint
 labels = lint
 allowlist_externals =
     shellcheck: bash, xargs
 commands_pre =
     shellcheck: bash -c '{[shellcheck]find} | {[shellcheck]filter} > {env_tmp_dir}/shellcheck_files'
 commands =
     black: black --check --diff {tty:--color} {posargs} .
+    codespell: codespell --toml {tox_root}/pyproject.toml {posargs}
+    rst: rstcheck {posargs:-r .}
     ruff: ruff check --respect-gitignore {posargs} .
     shellcheck: xargs -ra {env_tmp_dir}/shellcheck_files shellcheck
-    codespell: codespell --toml {tox_root}/pyproject.toml {posargs}
     yaml: yamllint {posargs} .
 
 [testenv:lint-{mypy,pyright}]
 description = Static type checking
 base = testenv, lint
 env_dir = {work_dir}/typing
 extras = dev, types
 labels = lint, type
 allowlist_externals =
     mypy: mkdir
 commands_pre =
     mypy: mkdir -p .mypy_cache
 commands =
     pyright: pyright {posargs}
-    mypy: mypy --install-types --non-interactive {posargs:.}
+    mypy: mypy --install-types --non-interactive {posargs:src tests}
 
 [testenv:format-{black,ruff,codespell}]
 description = Automatically format source code
 base = testenv, lint
 labels = format
 commands =
     black: black {tty:--color} {posargs} .
     ruff: ruff --fix --respect-gitignore {posargs} .
     codespell: codespell --toml {tox_root}/pyproject.toml --write-changes {posargs}
 
-[docs]  # Sphinx documentation configuration
-extras = docs
-package = editable
-no_package = true
-env_dir = {work_dir}/docs
-runner = ignore_env_name_mismatch
-
-[testenv:build-docs]
-description = Build sphinx documentation
-base = docs
-allowlist_externals = bash
-commands_pre = bash -c 'if [[ ! -e docs ]];then echo "No docs directory. Run `tox run -e sphinx-quickstart` to create one.;";return 1;fi'
-# "-W" is to treat warnings as errors
-commands = sphinx-build {posargs:-b html} -W {tox_root}/docs {tox_root}/docs/_build
-
-[testenv:autobuild-docs]
-description = Build documentation with an autoupdating server
-base = docs
-commands = sphinx-autobuild {posargs:-b html --open-browser --port 8080} -W --watch {tox_root}/starcraft {tox_root}/docs {tox_root}/docs/_build
-
-[testenv:lint-docs]
-description = Lint the documentation with sphinx-lint
-base = docs
-commands = sphinx-lint --ignore docs/_build --max-line-length 80 -e all {posargs} docs/
-labels = lint
+# [docs]  # Sphinx documentation configuration
+# extras = docs
+# package = editable
+# no_package = true
+# env_dir = {work_dir}/docs
+# runner = ignore_env_name_mismatch
+#
+# [testenv:build-docs]
+# description = Build sphinx documentation
+# base = docs
+# allowlist_externals = bash
+# commands_pre = bash -c 'if [[ ! -e docs ]];then echo "No docs directory. Run `tox run -e sphinx-quickstart` to create one.;";return 1;fi'
+# # "-W" is to treat warnings as errors
+# commands = sphinx-build {posargs:-b html} -W {tox_root}/docs {tox_root}/docs/_build
+#
+# [testenv:autobuild-docs]
+# description = Build documentation with an autoupdating server
+# base = docs
+# commands = sphinx-autobuild {posargs:-b html --open-browser --port 8080} -W --watch {tox_root}/starcraft {tox_root}/docs {tox_root}/docs/_build
+#
+# [testenv:lint-docs]
+# description = Lint the documentation with sphinx-lint
+# base = docs
+# commands = sphinx-lint --ignore docs/_build --max-line-length 80 -e all {posargs} docs/
+# labels = lint
```

