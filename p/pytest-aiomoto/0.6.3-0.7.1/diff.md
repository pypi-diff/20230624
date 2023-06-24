# Comparing `tmp/pytest_aiomoto-0.6.3.tar.gz` & `tmp/pytest_aiomoto-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_aiomoto-0.6.3.tar", max compression
+gzip compressed data, was "pytest_aiomoto-0.7.1.tar", max compression
```

## Comparing `pytest_aiomoto-0.6.3.tar` & `pytest_aiomoto-0.7.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0    11358 2022-10-29 02:11:15.595388 pytest_aiomoto-0.6.3/LICENSE
--rw-r--r--   0        0        0     4297 2022-11-09 05:14:50.343523 pytest_aiomoto-0.6.3/README.md
--rw-r--r--   0        0        0     2159 2022-11-09 05:14:50.340944 pytest_aiomoto-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      657 2022-11-09 04:11:03.821082 pytest_aiomoto-0.6.3/pytest_aiomoto/__init__.py
--rw-r--r--   0        0        0     6913 2022-11-09 04:11:03.821799 pytest_aiomoto-0.6.3/pytest_aiomoto/aiomoto_batch.py
--rw-r--r--   0        0        0     9890 2022-11-09 04:11:03.822204 pytest_aiomoto-0.6.3/pytest_aiomoto/aiomoto_fixtures.py
--rw-r--r--   0        0        0     2407 2022-11-09 04:11:03.823272 pytest_aiomoto-0.6.3/pytest_aiomoto/aiomoto_lambda.py
--rw-r--r--   0        0        0     4236 2022-11-09 04:11:03.823725 pytest_aiomoto-0.6.3/pytest_aiomoto/aiomoto_s3.py
--rw-r--r--   0        0        0     2620 2022-11-09 04:11:03.824112 pytest_aiomoto-0.6.3/pytest_aiomoto/aiomoto_s3fs.py
--rw-r--r--   0        0        0     3212 2022-11-09 04:11:03.824630 pytest_aiomoto-0.6.3/pytest_aiomoto/aiomoto_services.py
--rw-r--r--   0        0        0     7006 2022-11-09 04:11:03.825047 pytest_aiomoto-0.6.3/pytest_aiomoto/aws_batch.py
--rw-r--r--   0        0        0     2082 2022-11-09 04:30:23.592780 pytest_aiomoto-0.6.3/pytest_aiomoto/aws_batch_models.py
--rw-r--r--   0        0        0     4131 2022-11-09 04:11:03.827498 pytest_aiomoto-0.6.3/pytest_aiomoto/aws_clients.py
--rw-r--r--   0        0        0     1140 2022-11-09 04:11:03.828320 pytest_aiomoto-0.6.3/pytest_aiomoto/aws_cognito.py
--rw-r--r--   0        0        0    11230 2022-11-09 04:30:23.594391 pytest_aiomoto-0.6.3/pytest_aiomoto/aws_credentials.py
--rw-r--r--   0        0        0     1354 2022-11-09 04:11:03.829636 pytest_aiomoto-0.6.3/pytest_aiomoto/aws_host.py
--rw-r--r--   0        0        0     1597 2022-11-09 04:11:03.830979 pytest_aiomoto-0.6.3/pytest_aiomoto/aws_lambda.py
--rw-r--r--   0        0        0     2876 2022-11-09 04:11:03.832295 pytest_aiomoto-0.6.3/pytest_aiomoto/aws_regions.py
--rw-r--r--   0        0        0    14563 2022-11-09 04:11:03.832693 pytest_aiomoto-0.6.3/pytest_aiomoto/aws_s3.py
--rw-r--r--   0        0        0     4598 2022-11-09 04:11:03.833526 pytest_aiomoto-0.6.3/pytest_aiomoto/moto_services.py
--rw-r--r--   0        0        0     1282 2022-11-09 04:11:03.834109 pytest_aiomoto-0.6.3/pytest_aiomoto/plugin.py
--rw-r--r--   0        0        0     1449 2022-10-29 03:44:04.360540 pytest_aiomoto-0.6.3/pytest_aiomoto/s3_event.json
--rw-r--r--   0        0        0     1033 2022-11-09 04:11:03.834426 pytest_aiomoto-0.6.3/pytest_aiomoto/s3_object.py
--rw-r--r--   0        0        0     2849 2022-11-09 04:11:03.834752 pytest_aiomoto-0.6.3/pytest_aiomoto/utils.py
--rw-r--r--   0        0        0      861 2022-11-09 05:14:50.339172 pytest_aiomoto-0.6.3/pytest_aiomoto/version.py
--rw-r--r--   0        0        0     5528 1970-01-01 00:00:00.000000 pytest_aiomoto-0.6.3/setup.py
--rw-r--r--   0        0        0     5997 1970-01-01 00:00:00.000000 pytest_aiomoto-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-11-16 21:44:02.636432 pytest_aiomoto-0.7.1/LICENSE
+-rw-r--r--   0        0        0     4810 2023-06-24 21:02:11.039132 pytest_aiomoto-0.7.1/README.md
+-rw-r--r--   0        0        0     2238 2023-06-24 21:24:27.688552 pytest_aiomoto-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      657 2023-06-24 21:02:11.039986 pytest_aiomoto-0.7.1/pytest_aiomoto/__init__.py
+-rw-r--r--   0        0        0     6913 2023-06-24 21:02:11.040426 pytest_aiomoto-0.7.1/pytest_aiomoto/aiomoto_batch.py
+-rw-r--r--   0        0        0     9890 2023-06-24 21:02:11.040782 pytest_aiomoto-0.7.1/pytest_aiomoto/aiomoto_fixtures.py
+-rw-r--r--   0        0        0     2407 2023-06-24 21:02:11.041098 pytest_aiomoto-0.7.1/pytest_aiomoto/aiomoto_lambda.py
+-rw-r--r--   0        0        0     4236 2023-06-24 21:02:11.041416 pytest_aiomoto-0.7.1/pytest_aiomoto/aiomoto_s3.py
+-rw-r--r--   0        0        0     2620 2023-06-24 21:02:11.041732 pytest_aiomoto-0.7.1/pytest_aiomoto/aiomoto_s3fs.py
+-rw-r--r--   0        0        0     3212 2023-06-24 21:02:11.042048 pytest_aiomoto-0.7.1/pytest_aiomoto/aiomoto_services.py
+-rw-r--r--   0        0        0     7006 2023-06-24 21:02:11.042381 pytest_aiomoto-0.7.1/pytest_aiomoto/aws_batch.py
+-rw-r--r--   0        0        0     2082 2023-06-24 21:02:11.043127 pytest_aiomoto-0.7.1/pytest_aiomoto/aws_batch_models.py
+-rw-r--r--   0        0        0     4131 2023-06-24 21:02:11.043590 pytest_aiomoto-0.7.1/pytest_aiomoto/aws_clients.py
+-rw-r--r--   0        0        0     1140 2023-06-24 21:02:11.044089 pytest_aiomoto-0.7.1/pytest_aiomoto/aws_cognito.py
+-rw-r--r--   0        0        0    11230 2023-06-24 21:02:11.044500 pytest_aiomoto-0.7.1/pytest_aiomoto/aws_credentials.py
+-rw-r--r--   0        0        0     1354 2023-06-24 21:02:11.044835 pytest_aiomoto-0.7.1/pytest_aiomoto/aws_host.py
+-rw-r--r--   0        0        0     1597 2023-06-24 21:02:11.045175 pytest_aiomoto-0.7.1/pytest_aiomoto/aws_lambda.py
+-rw-r--r--   0        0        0     2876 2023-06-24 21:02:11.045493 pytest_aiomoto-0.7.1/pytest_aiomoto/aws_regions.py
+-rw-r--r--   0        0        0    14563 2023-06-24 21:02:11.045859 pytest_aiomoto-0.7.1/pytest_aiomoto/aws_s3.py
+-rw-r--r--   0        0        0     4598 2023-06-24 21:02:11.046336 pytest_aiomoto-0.7.1/pytest_aiomoto/moto_services.py
+-rw-r--r--   0        0        0     1282 2023-06-24 21:02:11.046798 pytest_aiomoto-0.7.1/pytest_aiomoto/plugin.py
+-rw-r--r--   0        0        0     1449 2022-11-16 21:44:02.641805 pytest_aiomoto-0.7.1/pytest_aiomoto/s3_event.json
+-rw-r--r--   0        0        0     1033 2023-06-24 21:02:11.047243 pytest_aiomoto-0.7.1/pytest_aiomoto/s3_object.py
+-rw-r--r--   0        0        0     2849 2023-06-24 21:02:11.047577 pytest_aiomoto-0.7.1/pytest_aiomoto/utils.py
+-rw-r--r--   0        0        0      676 2023-06-24 21:24:27.688960 pytest_aiomoto-0.7.1/pytest_aiomoto/version.py
+-rw-r--r--   0        0        0     6434 1970-01-01 00:00:00.000000 pytest_aiomoto-0.7.1/PKG-INFO
```

### Comparing `pytest_aiomoto-0.6.3/LICENSE` & `pytest_aiomoto-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_aiomoto-0.6.3/README.md` & `pytest_aiomoto-0.7.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -51,42 +51,59 @@
 Please review [github collaboration](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests)
 practices.  Once you clone your fork of the repository:
 
     cd pytest-aiomoto
     make init
     make test
 
+On OSX, use `gmake` from Homebrew to get GNU make > 4.x.
+
 It's recommended that development use python 3.8, to avoid introducing any python
 code that might not be compatible with the minimum version of python supported.  This
 is important in the context of the general evolution of asyncio in python.
 
 Most development is done in a linux context (e.g. Ubuntu LTS).  If some development
 tools or common practices are not working as expected on OSX or Windows, there is
 limited support for adapting to various development environments.
 
 Tests are run with [pytest](https://github.com/pytest-dev/pytest), please ensure
 the percentage of coverage at least stays the same before you submit a pull request.
 The expectation for contributions might be a slow process, please do not anticipate
 any turn around on the order of days (unless you're already a core contributor).
 Using your own fork can be a faster way to evolve your fixtures for your use cases.
 
+## Release Versions
+
+Install [pipx](https://pypa.github.io/pipx/) and use it to install
+[versionner](https://msztolcman.github.io/versionner/).
+
+```shell
+pipx install versionner
+ver --help
+```
+
+With `pipx` and `versionner` installed, it can be used to manage releases
+for any python library.  See the documentation for `ver` for details on
+how to manage sem-ver library releases.  See `.versionner.rc` file for
+details of the project configuration.
+
 ## Issues
 
 If you encounter any problems, please
 [file an issue](https://github.com/dazza-codes/pytest-aiomoto/issues)
 along with a detailed description.
 
 # License
 
 Distributed under the terms of the
 [Apache Software License 2.0](http://www.apache.org/licenses/LICENSE-2.0),
 "pytest-aiomoto" is free and open source software.
 
 ```text
-Copyright 2021 Darren Weber
+Copyright 2019-2023 Darren Weber
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pytest_aiomoto-0.6.3/pyproject.toml` & `pytest_aiomoto-0.7.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "pytest-aiomoto"
-version = "0.6.3"
+version = "0.7.1"
 description = "pytest-aiomoto"
 authors = [
     "Darren Weber <dazza-codes@github.com>",
 ]
 license = "Apache-2.0"
 
 readme = "README.md"
 repository = "https://github.com/dazza-codes/pytest-aiomoto.git"
 homepage = "https://github.com/dazza-codes/pytest-aiomoto"
 
 keywords = [
-    "Development Status :: 2 - Pre-Alpha",
-    "Intended Audience :: Developers",
-    "Operating System :: OS Independent",
+    "Development Status :: 3 - Alpha",
+    "Topic :: Software Development :: Testing",
     "Framework :: Pytest",
     "Intended Audience :: Developers",
-    "Topic :: Software Development :: Testing",
+    "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "License :: OSI Approved :: Apache Software License",
 ]
 
 include = ["pytest_aiomoto/**/*"]
 exclude = ["tests/**/*"]
 
@@ -40,53 +40,52 @@
 "aiomoto" = "pytest_aiomoto.plugin"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 pytest = "^7.0"
-pytest-asyncio = "^0.20"
+pytest-asyncio = "^0.21"
 
-# Allow updates to the latest aiobotocore and moto
-aiobotocore = {version = "^2.0.0", extras = ["boto3"]}
-moto = {version = "^4.0.0", extras = ["all","server"]}
+# Allow updates to the latest s3fs/aiobotocore and moto
+# Allow s3fs/aiobotcore to bundle compatible versions of botocore, boto3, and awscli;
+# see https://github.com/fsspec/s3fs/blob/main/setup.py
+s3fs = {version = "^2023.0", extras = ["awscli", "boto3"]}
+moto = {version = "^4.0", extras = ["all","server"]}
 
 aiofiles = "^22.0"
-requests = "^2.0.0"
-
-s3fs = {version = ">=0.5.0", optional = true}
+requests = "^2.0"
 
-mkdocs = {version = "^1.3.0", optional = true }
-mkdocs-material = {version = "^8.0.0", optional = true }
+mkdocs = {version = "^1.3", optional = true }
+mkdocs-material = {version = "^8.0", optional = true }
 mkdocstrings = {version = "^0.19.0", extras = ["python"], optional = true }
 
 
 [tool.poetry.extras]
 
 docs = [
     "mkdocs",
     "mkdocs-material",
     "mkdocstrings",
 ]
 
-s3fs = ["s3fs"]
 
 [tool.poetry.group.dev.dependencies]
 
 # py-dev-deps is used as a common denominator for many development dependencies
-py-dev-deps = "^0.5.0"
+py-dev-deps = "^0.5"
 
 # Add dev dependencies for testing projects with the
-# fixtures available from this project
-pandas = ">=1.0.0"
-zarr = ">=2.0.0"
-xarray = ">=0.20.2"
+# fixtures available from this project; see
+# tests/test_aio_s3fs.py
+pandas = "^1.0"
+zarr = "^2.0"
+xarray = "^2023.0"
 
 
 [tool.isort]
 profile = "black"
-force_single_line = true
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/__init__.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/aiomoto_batch.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/aiomoto_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/aiomoto_fixtures.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/aiomoto_fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/aiomoto_lambda.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/aiomoto_lambda.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/aiomoto_s3.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/aiomoto_s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/aiomoto_s3fs.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/aiomoto_s3fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/aiomoto_services.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/aiomoto_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/aws_batch.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/aws_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/aws_batch_models.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/aws_batch_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/aws_clients.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/aws_clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/aws_cognito.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/aws_cognito.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/aws_credentials.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/aws_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/aws_host.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/aws_host.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/aws_lambda.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/aws_lambda.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/aws_regions.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/aws_regions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/aws_s3.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/aws_s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/moto_services.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/moto_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/plugin.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/s3_event.json` & `pytest_aiomoto-0.7.1/pytest_aiomoto/s3_event.json`

 * *Files identical despite different names*

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/s3_object.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/s3_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/utils.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pytest_aiomoto-0.6.3/pytest_aiomoto/version.py` & `pytest_aiomoto-0.7.1/pytest_aiomoto/version.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-# Copyright 2019-2022 Darren Weber
+# Copyright 2019-2023 Darren Weber
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# pylint: disable=line-too-long
-# fmt: off
 """
-A version module managed by the invoke-release task
+A version module managed by versionner
 
-See also tasks.py
+See also .versionner.rc
 """
 
-__version_info__ = (0, 6, 3)
-__version__ = '-'.join(filter(None, ['.'.join(map(str, __version_info__[:3])), (__version_info__[3:] or [None])[0]]))
-# fmt: on
+__version__ = "0.7.1"
```

### Comparing `pytest_aiomoto-0.6.3/setup.py` & `pytest_aiomoto-0.7.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,151 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pytest-aiomoto
+Version: 0.7.1
+Summary: pytest-aiomoto
+Home-page: https://github.com/dazza-codes/pytest-aiomoto
+License: Apache-2.0
+Keywords: Development Status :: 3 - Alpha,Topic :: Software Development :: Testing,Framework :: Pytest,Intended Audience :: Developers,Operating System :: OS Independent,Programming Language :: Python,Programming Language :: Python :: 3,Programming Language :: Python :: 3.8,Programming Language :: Python :: 3.9,Programming Language :: Python :: 3.10,Programming Language :: Python :: 3.11,Programming Language :: Python :: 3 :: Only,License :: OSI Approved :: Apache Software License
+Author: Darren Weber
+Author-email: dazza-codes@github.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: docs
+Requires-Dist: aiofiles (>=22.0,<23.0)
+Requires-Dist: mkdocs (>=1.3,<2.0) ; extra == "docs"
+Requires-Dist: mkdocs-material (>=8.0,<9.0) ; extra == "docs"
+Requires-Dist: mkdocstrings[python] (>=0.19.0,<0.20.0) ; extra == "docs"
+Requires-Dist: moto[all,server] (>=4.0,<5.0)
+Requires-Dist: pytest (>=7.0,<8.0)
+Requires-Dist: pytest-asyncio (>=0.21,<0.22)
+Requires-Dist: requests (>=2.0,<3.0)
+Requires-Dist: s3fs[awscli,boto3] (>=2023.0,<2024.0)
+Project-URL: Repository, https://github.com/dazza-codes/pytest-aiomoto.git
+Description-Content-Type: text/markdown
+
+# pytest-aiomoto
+
+[![Build Status](https://github.com/dazza-codes/pytest-aiomoto/actions/workflows/python-test.yml/badge.svg)](https://github.com/dazza-codes/pytest-aiomoto/actions/workflows/python-test.yml)
+[![Documentation Status](https://readthedocs.org/projects/pytest-aiomoto/badge/?version=latest)](https://pytest-aiomoto.readthedocs.io/en/latest/?badge=latest)
+
+[![PyPI version](https://img.shields.io/pypi/v/pytest-aiomoto.svg)](https://pypi.org/project/pytest-aiomoto)
+[![Python versions](https://img.shields.io/pypi/pyversions/pytest-aiomoto.svg)](https://pypi.org/project/pytest-aiomoto)
+
+[pytest](https://docs.pytest.org) fixtures for AWS services,
+with support for asyncio fixtures using
+[aiobotocore](https://aiobotocore.readthedocs.io)
+
+## Warning
+
+- This package is work in progress, it is not recommended for production purposes.
+  During the initial phases of this project, it is likely that some releases
+  could introduce breaking changes in test fixtures.  It's highly
+  recommended pinning this dependency to patch releases during the
+  0.x.y releases.
+- This package could restrict available versions of aws libs, including:
+  aiobotocore, botocore, boto3, and moto.
+- The fixtures in this package might not be optimized for concurrent testing.
+  It is not known yet whether the fixtures are thread safe or adequately
+  randomized to support parallel test suites.
+
+## Installation
+
+You can install "pytest-aiomoto" via pip
+
+    $ pip install pytest-aiomoto
+
+## Usage
+
+To list the available fixtures
+
+    $ pytest --fixtures
+
+This project attempts to provide some common fixtures for commonly used
+services.  As such, it is not a generic package for any services; the
+moto project provides that and this project builds on that.  This
+project aims to create some useful fixtures that behave nearly the
+same way for both synchronous clients (botocore) and
+asynchronous clients (aiobotocore).
+
+## Contributing
+
+Contributions are welcome, if you build similar common fixtures or build
+on the existing package fixtures.  The details for bug fixes could be
+complicated, due to the dependencies on aiobotocore and moto.
+
+Please review [github collaboration](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests)
+practices.  Once you clone your fork of the repository:
+
+    cd pytest-aiomoto
+    make init
+    make test
+
+On OSX, use `gmake` from Homebrew to get GNU make > 4.x.
+
+It's recommended that development use python 3.8, to avoid introducing any python
+code that might not be compatible with the minimum version of python supported.  This
+is important in the context of the general evolution of asyncio in python.
+
+Most development is done in a linux context (e.g. Ubuntu LTS).  If some development
+tools or common practices are not working as expected on OSX or Windows, there is
+limited support for adapting to various development environments.
+
+Tests are run with [pytest](https://github.com/pytest-dev/pytest), please ensure
+the percentage of coverage at least stays the same before you submit a pull request.
+The expectation for contributions might be a slow process, please do not anticipate
+any turn around on the order of days (unless you're already a core contributor).
+Using your own fork can be a faster way to evolve your fixtures for your use cases.
+
+## Release Versions
+
+Install [pipx](https://pypa.github.io/pipx/) and use it to install
+[versionner](https://msztolcman.github.io/versionner/).
+
+```shell
+pipx install versionner
+ver --help
+```
+
+With `pipx` and `versionner` installed, it can be used to manage releases
+for any python library.  See the documentation for `ver` for details on
+how to manage sem-ver library releases.  See `.versionner.rc` file for
+details of the project configuration.
+
+## Issues
+
+If you encounter any problems, please
+[file an issue](https://github.com/dazza-codes/pytest-aiomoto/issues)
+along with a detailed description.
+
+# License
+
+Distributed under the terms of the
+[Apache Software License 2.0](http://www.apache.org/licenses/LICENSE-2.0),
+"pytest-aiomoto" is free and open source software.
+
+```text
+Copyright 2019-2023 Darren Weber
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+   http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+```
+
+# Notices
+
+Inspiration for this project comes from testing the
+[aio-aws](https://github.com/dazza-codes/aio-aws) project,
+which uses the Apache 2 license.
 
-packages = \
-['pytest_aiomoto']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiobotocore[boto3]>=2.0.0,<3.0.0',
- 'aiofiles>=22.0,<23.0',
- 'moto[all,server]>=4.0.0,<5.0.0',
- 'pytest-asyncio>=0.20,<0.21',
- 'pytest>=7.0,<8.0',
- 'requests>=2.0.0,<3.0.0']
-
-extras_require = \
-{'docs': ['mkdocs>=1.3.0,<2.0.0',
-          'mkdocs-material>=8.0.0,<9.0.0',
-          'mkdocstrings[python]>=0.19.0,<0.20.0'],
- 's3fs': ['s3fs>=0.5.0']}
-
-entry_points = \
-{'pytest11': ['aiomoto = pytest_aiomoto.plugin']}
-
-setup_kwargs = {
-    'name': 'pytest-aiomoto',
-    'version': '0.6.3',
-    'description': 'pytest-aiomoto',
-    'long_description': '# pytest-aiomoto\n\n[![Build Status](https://github.com/dazza-codes/pytest-aiomoto/actions/workflows/python-test.yml/badge.svg)](https://github.com/dazza-codes/pytest-aiomoto/actions/workflows/python-test.yml)\n[![Documentation Status](https://readthedocs.org/projects/pytest-aiomoto/badge/?version=latest)](https://pytest-aiomoto.readthedocs.io/en/latest/?badge=latest)\n\n[![PyPI version](https://img.shields.io/pypi/v/pytest-aiomoto.svg)](https://pypi.org/project/pytest-aiomoto)\n[![Python versions](https://img.shields.io/pypi/pyversions/pytest-aiomoto.svg)](https://pypi.org/project/pytest-aiomoto)\n\n[pytest](https://docs.pytest.org) fixtures for AWS services,\nwith support for asyncio fixtures using\n[aiobotocore](https://aiobotocore.readthedocs.io)\n\n## Warning\n\n- This package is work in progress, it is not recommended for production purposes.\n  During the initial phases of this project, it is likely that some releases\n  could introduce breaking changes in test fixtures.  It\'s highly\n  recommended pinning this dependency to patch releases during the\n  0.x.y releases.\n- This package could restrict available versions of aws libs, including:\n  aiobotocore, botocore, boto3, and moto.\n- The fixtures in this package might not be optimized for concurrent testing.\n  It is not known yet whether the fixtures are thread safe or adequately\n  randomized to support parallel test suites.\n\n## Installation\n\nYou can install "pytest-aiomoto" via pip\n\n    $ pip install pytest-aiomoto\n\n## Usage\n\nTo list the available fixtures\n\n    $ pytest --fixtures\n\nThis project attempts to provide some common fixtures for commonly used\nservices.  As such, it is not a generic package for any services; the\nmoto project provides that and this project builds on that.  This\nproject aims to create some useful fixtures that behave nearly the\nsame way for both synchronous clients (botocore) and\nasynchronous clients (aiobotocore).\n\n## Contributing\n\nContributions are welcome, if you build similar common fixtures or build\non the existing package fixtures.  The details for bug fixes could be\ncomplicated, due to the dependencies on aiobotocore and moto.\n\nPlease review [github collaboration](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests)\npractices.  Once you clone your fork of the repository:\n\n    cd pytest-aiomoto\n    make init\n    make test\n\nIt\'s recommended that development use python 3.8, to avoid introducing any python\ncode that might not be compatible with the minimum version of python supported.  This\nis important in the context of the general evolution of asyncio in python.\n\nMost development is done in a linux context (e.g. Ubuntu LTS).  If some development\ntools or common practices are not working as expected on OSX or Windows, there is\nlimited support for adapting to various development environments.\n\nTests are run with [pytest](https://github.com/pytest-dev/pytest), please ensure\nthe percentage of coverage at least stays the same before you submit a pull request.\nThe expectation for contributions might be a slow process, please do not anticipate\nany turn around on the order of days (unless you\'re already a core contributor).\nUsing your own fork can be a faster way to evolve your fixtures for your use cases.\n\n## Issues\n\nIf you encounter any problems, please\n[file an issue](https://github.com/dazza-codes/pytest-aiomoto/issues)\nalong with a detailed description.\n\n# License\n\nDistributed under the terms of the\n[Apache Software License 2.0](http://www.apache.org/licenses/LICENSE-2.0),\n"pytest-aiomoto" is free and open source software.\n\n```text\nCopyright 2021 Darren Weber\n\nLicensed under the Apache License, Version 2.0 (the "License");\nyou may not use this file except in compliance with the License.\nYou may obtain a copy of the License at\n\n   http://www.apache.org/licenses/LICENSE-2.0\n\nUnless required by applicable law or agreed to in writing, software\ndistributed under the License is distributed on an "AS IS" BASIS,\nWITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\nSee the License for the specific language governing permissions and\nlimitations under the License.\n```\n\n# Notices\n\nInspiration for this project comes from testing the\n[aio-aws](https://github.com/dazza-codes/aio-aws) project,\nwhich uses the Apache 2 license.\n',
-    'author': 'Darren Weber',
-    'author_email': 'dazza-codes@github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/dazza-codes/pytest-aiomoto',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

